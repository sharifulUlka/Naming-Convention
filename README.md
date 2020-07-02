## C# Naming Convention

<table>

<!-- New Table Row -->
<tr>
<td>
   <p>Types and Namespaces</p>
</td>
<td>
  <p>UpperCamelCase</p>
</td>
<td>
  <details>
    <summary>Show code</summary>
      <pre lang="csharp">
public namespace AddaNameSpace
{
    public class AddaGameManager { }
    public struct GameData { }
}</pre>
    </details>
</td>
</tr>

<!-- New Table Row -->
<tr>
<td>
   <p>Interfaces</p>
</td>
<td>
  <p>IUpperCamelCase</p>
</td>
<td>
  <details>
    <summary>Show code</summary>
      <pre lang="csharp">
public interface IAddaGame
{
    // Interface stuff
}</pre>
    </details>
</td>
</tr>


<!-- New Table Row -->
<tr>
<td>
   <p>Methods</p>
</td>
<td>
  <p>UpperCamelCase</p>
</td>
<td>
  <details>
    <summary>Show code</summary>
      <pre lang="csharp">
public void DoStuff()
{
    // Method body
}
</pre>
    </details>
</td>
</tr>

<!-- New Table Row -->
<tr>
<td>
   <p>Properties</p>
</td>
<td>
  <p>UpperCamelCase</p>
</td>
<td>
  <details>
    <summary>Show code</summary>
      <pre lang="csharp">
public class Player : MonoBehaviour 
{
    public int PlayerSpeed 
    {
        get { return _speed; }
        set { _speed = ValidateSpeed(value); }
    }
...
}
</pre>
    </details>
</td>
</tr>

<!-- New Table Row -->
<tr>
<td>
   <p>Events</p>
</td>
<td>
  <p>UpperCamelCase</p>
</td>
<td>
  <details>
    <summary>Show code</summary>
      <pre lang="csharp">
public class Player : MonoBehaviour
{
    public event EventHandler OnPlayerPrepared;
}
</pre>
    </details>
</td>
</tr>
<!-- New Table Row -->
<tr>
<td>
   <p>Unity Serialized Fields</p>
</td>
<td>
  <p>m_UpperCamelCase</p>
</td>
<td>
  <details>
    <summary>Show code</summary>
      <pre lang="csharp">
public class Player : Monobehaviour 
{
    [SerializedField] private int m_Speed;
    public int m_Velocity;
    [HideInInspector] public RigidBody RigidBodyComponent;

...
}
</pre>
    </details>
</td>
</tr>

<!-- New Table Row -->
<tr>
<td>
   <p>Fields (Not Private)</p>
</td>
<td>
  <p>UpperCamelCase</p>
</td>
<td>
  <details>
    <summary>Show code</summary>
      <pre lang="csharp">
public class Player
{
    public static int Speed;
    public int Balance;
    internal string PlayerName;
    protected string PlayerId;
}
</pre>
    </details>
</td>
</tr>

<!-- New Table Row -->
<tr>
<td>
   <p>Fields (Private)</p>
</td>
<td>
  <p>_lowerCamelCase</p>
</td>
<td>
  <details>
    <summary>Show code</summary>
      <pre lang="csharp">
public class Player
{
    private static int _speed;
    private int _balance; 
}
</pre>
    </details>
</td>
</tr>

<!-- New Table Row -->
<tr>
<td>
   <p>Constant Fields (Private/Not Private)</p>
</td>
<td>
  <p>UpperCamelCase</p>
</td>
<td>
  <details>
    <summary>Show code</summary>
      <pre lang="csharp">
public class Player
{
    private const int PlayerCount;
    public const int Balance;
    internal const string PlayerName;
    protected const string PlayerId;
}
</pre>
    </details>
</td>
</tr>

<!-- New Table Row -->
<tr>
<td>
   <p>Parameters</p>
</td>
<td>
  <p>lowerCamelCase</p>
</td>
<td>
  <details>
    <summary>Show code</summary>
      <pre lang="csharp">
public class Player : MonoBehaviour
{
    private void DoStuff(int stuffCount)
    {
        ...
    }
...
}
</pre>
    </details>
</td>
</tr>

<!-- New Table Row -->
<tr>
<td>
   <p>Type Parameters</p>
</td>
<td>
  <p>TUpperCamelCase</p>
</td>
<td>
  <details>
    <summary>Show code</summary>
      <pre lang="csharp">
public void DoStuff(Type TPlayer) { }
</pre>
    </details>
</td>
</tr>

<!-- New Table Row -->
<tr>
<td>
   <p>Local variables, Local Constants</p>
</td>
<td>
  <p>lowerCamelCase</p>
</td>
<td>
  <details>
    <summary>Show code</summary>
      <pre lang="csharp">
public class Player : MonoBehaviour
{
    private void DoStuff()
    {
        int stuffCount;
        const char stuffChar;
        ...
    }
...
}
</pre>
    </details>
</td>
</tr>

<!-- New Table Row -->
<tr>
<td>
   <p>Enum Members</p>
</td>
<td>
  <p>ALL_UPPER</p>
</td>
<td>
  <details>
    <summary>Show code</summary>
      <pre lang="csharp">
enum EnemyType
{
    RANGED = 0,
    MELE, 
    SHORT_HANDED
}
</pre>
    </details>
</td>
</tr>
