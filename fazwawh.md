代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://kx.zhonguo7118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://zh.zhonguo7118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://dj.zhonguo5118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://ie.zhonguo7118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://ow.zhonguo3118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://om.zhonguo4118.cn

[E16] 数字千分位
来源：https://oy.zhonguo6118.cn

Py:   f"{1234567:,}"
来源：https://wy.zhonguo7118.cn

PHP:  number_format(1234567);
来源：https://ai.zhonguo2118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://xg.zhonguo3118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://xo.zhonguo8118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://bz.zhonguo2118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://ly.zhonguo4118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://br.zhonguo7118.cn

C#:   1234567.ToString("N0")
来源：https://ne.zhonguo2118.cn

[E17] 首字母大写
来源：https://vo.zhonguo5118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://se.zhonguo6118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://tn.zhonguo7118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://vk.zhonguo1118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://sv.zhonguo4118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://ou.zhonguo4118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://es.zhonguo3118.cn

Ruby: s.capitalize
来源：https://fi.zhonguo6118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://cf.zhonguo8118.cn

[E18] 模板占位符替换
来源：https://ru.zhonguo3118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://em.zhonguo1118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://ec.zhonguo4118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://wm.zhonguo2118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://bv.zhonguo8118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://vb.zhonguo3118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://mv.zhonguo5118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://kd.zhonguo5118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://nr.zhonguo3118.cn

[E19] 多行文本按行拆分
来源：https://kj.zhonguo6118.cn

Py:   s.splitlines()
来源：https://hv.zhonguo1118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://zs.zhonguo4118.cn

JS:   s.split(/\r?\n/)
来源：https://jz.zhonguo4118.cn

TS:   s.split(/\r?\n/)
来源：https://fv.zhonguo4118.cn

Java: s.lines().toList()
来源：https://mo.zhonguo3118.cn

Go:   strings.Split(s, "\n")
来源：https://ti.zhonguo5118.cn

Ruby: s.lines
来源：https://jp.zhonguo4118.cn

C#:   s.Split('\n')
来源：https://er.zhonguo2118.cn

[E20] 判断字符串是否为空
来源：https://ob.zhonguo7118.cn

Py:   if not s:
来源：https://lo.zhonguo5118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://ar.zhonguo7118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://bu.zhonguo3118.cn

TS:   if (s === "") {}
来源：https://fz.zhonguo1118.cn

Java: if (s.isEmpty()) {}
来源：https://ex.zhonguo4118.cn

Go:   if s == "" {}
来源：https://lg.zhonguo6118.cn

Ruby: if s.empty?
来源：https://oj.zhonguo6118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://hr.zhonguo3118.cn

[E21] 超长截断加省略号
来源：https://hk.zhonguo3118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://rp.zhonguo7118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://ot.zhonguo5118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://df.zhonguo6118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://lh.zhonguo2118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://on.zhonguo2118.cn

Go:   // 按 rune 判断长度后截断
来源：https://zd.zhonguo3118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://mt.zhonguo5118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://ki.zhonguo3118.cn

[E22] 字节长度与字符长度
来源：https://wd.zhonguo4118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://xq.zhonguo3118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://tz.zhonguo2118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://ll.zhonguo6118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://lf.zhonguo2118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://ud.zhonguo8118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://oc.zhonguo4118.cn

Ruby: s.bytesize;  s.length
来源：https://yz.zhonguo7118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://mx.zhonguo2118.cn

================================================================================
来源：https://ao.zhonguo4118.cn

F. 文件与目录
来源：https://yo.zhonguo5118.cn

================================================================================
来源：https://wz.zhonguo6118.cn

[F01] 读取整个文件
来源：https://zk.zhonguo6118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://ep.zhonguo7118.cn

PHP:  file_get_contents("a.txt");
来源：https://de.zhonguo8118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://oa.zhonguo4118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://vg.zhonguo8118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://dh.zhonguo4118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://ob.zhonguo6118.cn

Ruby: File.read("a.txt")
来源：https://tk.zhonguo8118.cn

C#:   File.ReadAllText("a.txt");
来源：https://be.zhonguo5118.cn

[F02] 逐行读取文件
来源：https://uz.zhonguo2118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://gn.zhonguo6118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://jz.zhonguo4118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://dy.zhonguo3118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://ap.zhonguo2118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://rm.zhonguo6118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://hk.zhonguo8118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://un.zhonguo1118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://gh.zhonguo5118.cn

[F03] 写入文件（覆盖）
来源：https://ii.zhonguo2118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://lp.zhonguo4118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://tc.zhonguo4118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://tq.zhonguo7118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://qc.zhonguo3118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://ae.zhonguo3118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://al.zhonguo7118.cn

Ruby: File.write("a.txt", "hi")
来源：https://gn.zhonguo3118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://ji.zhonguo1118.cn

[F04] 追加写入文件
来源：https://sk.zhonguo3118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://gv.zhonguo5118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://wv.zhonguo7118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://fr.zhonguo7118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://kg.zhonguo2118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://ut.zhonguo8118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://bv.zhonguo8118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://hr.zhonguo6118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://tg.zhonguo2118.cn

[F05] 判断文件或目录是否存在
来源：https://mu.zhonguo8118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://ut.zhonguo1118.cn

PHP:  file_exists("a.txt");
来源：https://xq.zhonguo3118.cn

JS:   fs.existsSync("a.txt")
来源：https://wg.zhonguo6118.cn

TS:   fs.existsSync("a.txt")
来源：https://pz.zhonguo7118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://cz.zhonguo3118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://el.zhonguo4118.cn

Ruby: File.exist?("a.txt")
来源：https://wk.zhonguo2118.cn

C#:   File.Exists("a.txt")
来源：https://mn.zhonguo3118.cn

[F06] 删除文件
来源：https://af.zhonguo8118.cn

Py:   os.remove("a.txt")
来源：https://dr.zhonguo8118.cn

PHP:  unlink("a.txt");
来源：https://ql.zhonguo8118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://ci.zhonguo1118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://ks.zhonguo6118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://js.zhonguo1118.cn

Go:   os.Remove("a.txt")
来源：https://zk.zhonguo5118.cn

Ruby: File.delete("a.txt")
来源：https://pf.zhonguo8118.cn

C#:   File.Delete("a.txt");
来源：https://jh.zhonguo5118.cn

[F07] 创建目录（含多级）
来源：https://qo.zhonguo7118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://pe.zhonguo1118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://qs.zhonguo3118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://qy.zhonguo8118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://op.zhonguo8118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://ef.zhonguo2118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://th.zhonguo2118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://ag.zhonguo7118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://vo.zhonguo2118.cn

[F08] 遍历目录
来源：https://gn.zhonguo3118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://om.zhonguo8118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://eh.zhonguo8118.cn

JS:   fs.readdirSync("dir")
来源：https://nv.zhonguo8118.cn

TS:   fs.readdirSync("dir")
来源：https://if.zhonguo8118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://qz.zhonguo2118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://pv.zhonguo4118.cn

Ruby: Dir.children("dir")
来源：https://je.zhonguo2118.cn

C#:   Directory.GetFiles("dir")
来源：https://gn.zhonguo3118.cn

[F09] 获取文件大小
来源：https://dg.zhonguo4118.cn

Py:   os.path.getsize("a.txt")
来源：https://ec.zhonguo8118.cn

PHP:  filesize("a.txt");
来源：https://rv.zhonguo7118.cn

JS:   fs.statSync("a.txt").size
来源：https://jk.zhonguo1118.cn

TS:   fs.statSync("a.txt").size
来源：https://ir.zhonguo2118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://ph.zhonguo2118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://dp.zhonguo8118.cn

Ruby: File.size("a.txt")
来源：https://zp.zhonguo2118.cn

C#:   new FileInfo("a.txt").Length
来源：https://mv.zhonguo7118.cn

[F10] 取文件扩展名 / 文件名
来源：https://ll.zhonguo7118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://il.zhonguo3118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://hk.zhonguo2118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://hs.zhonguo2118.cn

TS:   path.extname("a.txt")
来源：https://by.zhonguo2118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://au.zhonguo4118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://io.zhonguo2118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://ar.zhonguo5118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://sl.zhonguo1118.cn

[F11] 复制与移动文件
来源：https://yi.zhonguo8118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://ys.zhonguo2118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://qq.zhonguo5118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://je.zhonguo5118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://by.zhonguo8118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://ar.zhonguo3118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://up.zhonguo3118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://zi.zhonguo8118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://br.zhonguo6118.cn

[F12] CSV 读写
来源：https://py.zhonguo1118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://ga.zhonguo2118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://ps.zhonguo8118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://ct.zhonguo7118.cn

TS:   // 同上
来源：https://mv.zhonguo7118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://oa.zhonguo8118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://wt.zhonguo7118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://xx.zhonguo4118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://zy.zhonguo4118.cn

================================================================================
来源：https://al.zhonguo5118.cn

G. 面向对象
来源：https://jd.zhonguo2118.cn

================================================================================
来源：https://rv.zhonguo4118.cn

[G01] 定义类
来源：https://nl.zhonguo8118.cn

Py:   class User: pass
来源：https://be.zhonguo2118.cn

PHP:  class User {}
来源：https://je.zhonguo5118.cn

JS:   class User {}
来源：https://ka.zhonguo8118.cn

TS:   class User { name: string = ""; }
来源：https://fd.zhonguo6118.cn

Java: class User {}
来源：https://tf.zhonguo2118.cn

Go:   type User struct { Name string }
来源：https://iv.zhonguo4118.cn

Ruby: class User; end
来源：https://xf.zhonguo4118.cn

C#:   class User {}
来源：https://xe.zhonguo2118.cn

[G02] 构造函数
来源：https://oj.zhonguo7118.cn

Py:   def __init__(self, name): self.name = name
来源：https://lp.zhonguo5118.cn

PHP:  public function __construct(public string $name) {}
来源：https://ts.zhonguo4118.cn

JS:   constructor(name) { this.name = name; }
来源：https://av.zhonguo7118.cn

TS:   constructor(public name: string) {}
来源：https://ks.zhonguo1118.cn

Java: User(String name) { this.name = name; }
来源：https://bo.zhonguo3118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://dh.zhonguo7118.cn

Ruby: def initialize(name); @name = name; end
来源：https://pe.zhonguo7118.cn

C#:   public User(string name) { Name = name; }
来源：https://ta.zhonguo1118.cn

[G03] 实例属性
来源：https://ce.zhonguo8118.cn

Py:   self.name = "x"
来源：https://iq.zhonguo2118.cn

PHP:  public string $name = "x";
来源：https://fz.zhonguo8118.cn

JS:   this.name = "x";
来源：https://dg.zhonguo6118.cn

TS:   name: string = "x";
来源：https://qm.zhonguo7118.cn

Java: private String name;
来源：https://bo.zhonguo3118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://ns.zhonguo5118.cn

Ruby: @name = "x"
来源：https://ty.zhonguo5118.cn

C#:   public string Name { get; set; } = "x";
来源：https://by.zhonguo5118.cn

[G04] 定义方法
来源：https://or.zhonguo1118.cn

Py:   def greet(self): return self.name
来源：https://qs.zhonguo8118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://xj.zhonguo1118.cn

JS:   greet() { return this.name; }
来源：https://jx.zhonguo7118.cn

TS:   greet(): string { return this.name; }
来源：https://pb.zhonguo4118.cn

Java: String greet() { return name; }
来源：https://ik.zhonguo8118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://dp.zhonguo4118.cn

Ruby: def greet; @name; end
来源：https://kn.zhonguo1118.cn

C#:   public string Greet() => Name;
来源：https://ak.zhonguo2118.cn

[G05] 继承
来源：https://ge.zhonguo1118.cn

Py:   class Admin(User): pass
来源：https://pw.zhonguo1118.cn

PHP:  class Admin extends User {}
来源：https://wu.zhonguo7118.cn

JS:   class Admin extends User {}
来源：https://vf.zhonguo8118.cn

TS:   class Admin extends User {}
来源：https://fm.zhonguo6118.cn

Java: class Admin extends User {}
来源：https://tq.zhonguo2118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://db.zhonguo2118.cn

Ruby: class Admin < User; end
来源：https://jb.zhonguo3118.cn

C#:   class Admin : User {}
来源：https://oq.zhonguo3118.cn

[G06] 重写方法
来源：https://kz.zhonguo2118.cn

Py:   def greet(self): return "admin"
来源：https://sm.zhonguo1118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://hg.zhonguo3118.cn

JS:   greet() { return "admin"; }
来源：https://hk.zhonguo7118.cn

TS:   greet(): string { return "admin"; }
来源：https://kw.zhonguo1118.cn

Java: @Override String greet() { return "admin"; }
来源：https://ja.zhonguo6118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://cj.zhonguo2118.cn

Ruby: def greet; "admin"; end
来源：https://tn.zhonguo7118.cn

C#:   public override string Greet() => "admin";
来源：https://cq.zhonguo2118.cn

[G07] 调用父类方法
来源：https://fy.zhonguo7118.cn

Py:   super().greet()
来源：https://ut.zhonguo7118.cn

PHP:  parent::greet();
来源：https://ri.zhonguo6118.cn

JS:   super.greet();
来源：https://bt.zhonguo1118.cn

TS:   super.greet();
来源：https://cm.zhonguo2118.cn

Java: super.greet();
来源：https://gr.zhonguo4118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://dw.zhonguo4118.cn

Ruby: super
来源：https://qn.zhonguo3118.cn

C#:   base.Greet();
来源：https://wo.zhonguo7118.cn

[G08] 静态方法与属性
来源：https://tl.zhonguo7118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://gu.zhonguo6118.cn

PHP:  public static function f() {}
来源：https://nu.zhonguo4118.cn

JS:   static f() {}
来源：https://tf.zhonguo4118.cn

TS:   static f(): void {}
来源：https://sb.zhonguo4118.cn

Java: static void f() {}
来源：https://xb.zhonguo3118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://sd.zhonguo4118.cn

Ruby: def self.f; end
来源：https://fw.zhonguo6118.cn

C#:   public static void F() {}
来源：https://li.zhonguo6118.cn

[G09] 接口 / 抽象类
来源：https://lh.zhonguo4118.cn

Py:   from abc import ABC, abstractmethod
来源：https://yx.zhonguo6118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://pe.zhonguo8118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://pj.zhonguo5118.cn

TS:   interface Shape { area(): number; }
来源：https://vt.zhonguo1118.cn

Java: interface Shape { double area(); }
来源：https://ea.zhonguo5118.cn

Go:   type Shape interface { Area() float64 }
来源：https://wo.zhonguo2118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://wg.zhonguo2118.cn

C#:   interface IShape { double Area(); }
来源：https://lm.zhonguo2118.cn

[G10] 访问控制
来源：https://rn.zhonguo4118.cn

Py:   约定 _protected / __private（不强制）
来源：https://gu.zhonguo7118.cn

PHP:  public / protected / private
来源：https://yb.zhonguo8118.cn

JS:   #private 字段；其余公开
来源：https://sa.zhonguo8118.cn

TS:   public / protected / private
来源：https://sn.zhonguo5118.cn

Java: public / protected / private / 默认包级
来源：https://jt.zhonguo2118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://gw.zhonguo4118.cn

Ruby: public / protected / private
来源：https://fs.zhonguo5118.cn

C#:   public / protected / private / internal
来源：https://za.zhonguo4118.cn

[G11] getter / setter
来源：https://pn.zhonguo8118.cn

Py:   @property 与 @x.setter
来源：https://zi.zhonguo5118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://cp.zhonguo6118.cn

JS:   get name() { return this._name; }
来源：https://ix.zhonguo5118.cn

TS:   get name(): string { return this._name; }
来源：https://wq.zhonguo7118.cn

Java: public String getName() { return name; }
来源：https://xe.zhonguo2118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://ft.zhonguo2118.cn

Ruby: attr_accessor :name
来源：https://bt.zhonguo7118.cn

C#:   public string Name { get; set; }
来源：https://qh.zhonguo4118.cn

[G12] 对象转字符串
来源：https://vn.zhonguo6118.cn

Py:   def __str__(self): return self.name
来源：https://qk.zhonguo3118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://so.zhonguo6118.cn

JS:   toString() { return this.name; }
来源：https://ca.zhonguo7118.cn

TS:   toString(): string { return this.name; }
来源：https://dt.zhonguo4118.cn

Java: @Override public String toString() { return name; }
来源：https://yt.zhonguo3118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://hb.zhonguo3118.cn

Ruby: def to_s; @name; end
来源：https://qz.zhonguo8118.cn

C#:   public override string ToString() => Name;
来源：https://jy.zhonguo8118.cn

[G13] 判断对象类型
来源：https://bs.zhonguo3118.cn

Py:   isinstance(u, User)
来源：https://dp.zhonguo7118.cn

PHP:  $u instanceof User
来源：https://dh.zhonguo4118.cn

JS:   u instanceof User
来源：https://ab.zhonguo7118.cn

TS:   u instanceof User
来源：https://re.zhonguo8118.cn

Java: u instanceof User
来源：https://wr.zhonguo6118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://aj.zhonguo6118.cn

Ruby: u.is_a?(User)
来源：https://pv.zhonguo5118.cn

C#:   u is User
来源：https://ae.zhonguo4118.cn


<!-- 参考信息 -->