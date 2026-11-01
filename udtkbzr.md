代发 wailian999

Ruby: attr_accessor :name
来源：http://www.share.bbcook.cn/Article/details/gfuooumvi.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fktsv.cn/Article/details/gwqvurbcy.sHtML

[G12] 对象转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gmtpnrdxr.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gloqgbbhm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gtolsomuq.sHtML

JS:   toString() { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gtlhnvrsm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gotnvlteb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gywufplzi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/ghzthhpon.sHtML

Ruby: def to_s; @name; end
来源：http://wap.epnwcf.com/Article/details/gjigeipzx.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fktsv.cn/Article/details/gdrkhuzfd.sHtML

[G13] 判断对象类型
来源：http://www.m.share.vehdjk.com/Article/details/gbpdpybzw.sHtML

Py:   isinstance(u, User)
来源：http://www.share.vehdjk.com/Article/details/gagekbiqx.sHtML

PHP:  $u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gffglcygj.sHtML

JS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gewnizpad.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gobuuquni.sHtML

Java: u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gagmnxyab.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/gndvtfywd.sHtML

Ruby: u.is_a?(User)
来源：http://3g.vehdjk.com/Article/details/gxtmtgegx.sHtML

C#:   u is User
来源：http://baike.tarul.cn/Article/details/gabagvidc.sHtML

[G14] 数据类 / record
来源：http://m.share.epnwcf.com/Article/details/gvovzfesl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/gvpkyxnxq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.tarul.cn/Article/details/gmmmqfxos.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.vehdjk.com/Article/details/gbyybbyhh.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fktsv.cn/Article/details/gpaqgwajk.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fktsv.cn/Article/details/gvxufhsvd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.bbcook.cn/Article/details/gegbwkhgm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.tarul.cn/Article/details/gobmpgorv.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fktsv.cn/Article/details/gqngsyyda.sHtML

[G15] 枚举
来源：http://3g.tarul.cn/Article/details/gfsrhdvhd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/glozgvbtt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fktsv.cn/Article/details/guagkwxik.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.vehdjk.com/Article/details/geyifddro.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gqzaxsuwo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/gwcvrsokg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fktsv.cn/Article/details/garqhfexo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbmwcegh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/guxlyttor.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.epnwcf.com/Article/details/gqszdhtpt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.sjlbkw.cn/Article/details/gxoegpkbb.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.yfazqb.com/Article/details/gxjteddfw.sHtML

JS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gajgovjsy.sHtML

TS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gnenqxmzh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.vehdjk.com/Article/details/gscztrfdb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fktsv.cn/Article/details/gwpvjnfgl.sHtML

Ruby: obj.instance_variables
来源：http://m.share.vehdjk.com/Article/details/gynuvrtns.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/gdjmcqcpv.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpomxwkmy.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gctubkiik.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmhuhlqhi.sHtML

[H01] try / catch 基础
来源：http://3g.yfazqb.com/Article/details/gyqpwrbtr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.yfazqb.com/Article/details/gmlvmnwva.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.vehdjk.com/Article/details/gpzplnxwf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/ggwjdfvdn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gxixbqjsw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.epnwcf.com/Article/details/gejtfqbwa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.epnwcf.com/Article/details/gntsvachz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fktsv.cn/Article/details/gvjaouwim.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.epnwcf.com/Article/details/gmekfivgq.sHtML

[H02] finally / ensure 收尾
来源：http://blog.epnwcf.com/Article/details/gkgsygncy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fktsv.cn/Article/details/gounwwkda.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/glqouzbce.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gprijfojm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/geetrifcf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gctsqbzhj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.tarul.cn/Article/details/gfpyiwklj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.bbcook.cn/Article/details/gaqnisnqd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.tarul.cn/Article/details/gdnqppwni.sHtML

[H03] 主动抛出异常
来源：http://baike.tarul.cn/Article/details/gkpyiibww.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.tarul.cn/Article/details/ggtaybpvs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gryqypelk.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/gohlpiunm.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gjwzvzazd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gnhyipnuh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.sjlbkw.cn/Article/details/gkjwflboi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.sjlbkw.cn/Article/details/guuvjrhrl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gvoexmgrn.sHtML

[H04] 自定义异常类型
来源：http://mobile.yfazqb.com/Article/details/gadcvngrx.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.bbcook.cn/Article/details/gaexhxgtg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gxvykgjan.sHtML

JS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gwsztimqr.sHtML

TS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/gxujzcvmq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gxezzxvcb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.sjlbkw.cn/Article/details/gwnznreau.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.yfazqb.com/Article/details/gpstadyjh.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gdquvmtwk.sHtML

[H05] 捕获特定类型
来源：http://wap.epnwcf.com/Article/details/gnzrbxlfj.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.tarul.cn/Article/details/gxgqzhzhe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.epnwcf.com/Article/details/gnnkllgsk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/gkalkdyji.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gnouwapqw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.tarul.cn/Article/details/gulefkprh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fktsv.cn/Article/details/grcvvgdqq.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/ghdybwxcp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.vehdjk.com/Article/details/gakdkyyfa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.epnwcf.com/Article/details/gnhtnetfh.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.yfazqb.com/Article/details/gtubbvoya.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gwrbxbizz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fktsv.cn/Article/details/gabjvwfaq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gmufzfgzd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.tarul.cn/Article/details/gygzrlkre.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.vehdjk.com/Article/details/gunkcpbic.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.bbcook.cn/Article/details/gabwfcxyn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.tarul.cn/Article/details/gjakqfiqp.sHtML

[H07] 断言
来源：http://mobile.epnwcf.com/Article/details/giemcurco.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.bbcook.cn/Article/details/gcnnvfvwl.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gcqqrrwge.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gyhlqoqpx.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/giunmmoao.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.bbcook.cn/Article/details/gvxsilyhl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.yfazqb.com/Article/details/gixibowrv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.epnwcf.com/Article/details/gwvndxcom.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/ghosmqlkk.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.vehdjk.com/Article/details/gmealnpqj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fktsv.cn/Article/details/gcstmrcsv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fktsv.cn/Article/details/gzveoovvg.sHtML

JS:   e.message;  e.stack
来源：http://wap.bbcook.cn/Article/details/gwwmkvlyt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.bbcook.cn/Article/details/gddxilwty.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.yfazqb.com/Article/details/ghfywrrev.sHtML

Go:   err.Error()
来源：http://www.m.share.epnwcf.com/Article/details/ggxhderpw.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/gogmjttku.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.vehdjk.com/Article/details/gwygwhjvk.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/ghuvjcfmg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.yfazqb.com/Article/details/ghgzhhnvf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.yfazqb.com/Article/details/ggetgohkc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.bbcook.cn/Article/details/gviewarzt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.bbcook.cn/Article/details/gqlftnekl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fktsv.cn/Article/details/ganxetcaq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.bbcook.cn/Article/details/gteurkinz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.tarul.cn/Article/details/gikyfgejh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.bbcook.cn/Article/details/ggjvtmofo.sHtML

[H10] 资源自动释放
来源：http://mobile.vehdjk.com/Article/details/gbsvwotqy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.bbcook.cn/Article/details/gslbgyrwf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fktsv.cn/Article/details/ggvjbahdv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/getuyiink.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gopuiyrwv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.tarul.cn/Article/details/gbockzyam.sHtML

Go:   defer f.Close()
来源：http://mobile.bbcook.cn/Article/details/glitpwxkw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.epnwcf.com/Article/details/gdaptptpf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fktsv.cn/Article/details/gqbdhrpnc.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gujofmcgs.sHtML

I. 正则表达式
来源：http://wap.bbcook.cn/Article/details/gxgiideug.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggfzpjxiw.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gfbjhyssu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.tarul.cn/Article/details/gmvlxmlxj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.tarul.cn/Article/details/gazbrgfya.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gijzcubei.sHtML

TS:   /\d+/.test(s)
来源：http://baike.epnwcf.com/Article/details/gcgzphhtq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.bbcook.cn/Article/details/gnsvewojb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.tarul.cn/Article/details/gbcbhfhho.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gmodllbob.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.tarul.cn/Article/details/grhmjdygy.sHtML

[I02] 提取所有匹配
来源：http://www.share.vehdjk.com/Article/details/gaqryidzp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/glqqdkcbn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/gdycuwepg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.tarul.cn/Article/details/gffyvhpql.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.yfazqb.com/Article/details/gnwxzdmvm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.yfazqb.com/Article/details/gbjevidar.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gthlluosk.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gsbjtdbpc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.epnwcf.com/Article/details/geajhjglg.sHtML

[I03] 提取捕获分组
来源：http://www.blog.tarul.cn/Article/details/gbyjtlhgb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.epnwcf.com/Article/details/ghizgseuk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.bbcook.cn/Article/details/gzhjefenv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.bbcook.cn/Article/details/gvfygivwl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.vehdjk.com/Article/details/greypiowm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fktsv.cn/Article/details/gqnaeifcf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.sjlbkw.cn/Article/details/gtytxjrxv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.tarul.cn/Article/details/gkowqxoif.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.tarul.cn/Article/details/gmstioaoj.sHtML

[I04] 正则替换
来源：http://www.m.share.epnwcf.com/Article/details/gxdpptspu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.epnwcf.com/Article/details/gtkigqonq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/gxwcjnecc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/ghyjykear.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfebnlhyy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/glxqdgeqo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.epnwcf.com/Article/details/gfxnbuqkp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/goywnpkam.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gmiykinxm.sHtML

[I05] 按正则拆分
来源：http://m.share.fktsv.cn/Article/details/grthavcbb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.tarul.cn/Article/details/gmehrekws.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/goaeuxyof.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gwilrsrcj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gbvrpwyoy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.yfazqb.com/Article/details/gcfcowepu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gwcriztrw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gybdrtudc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.bbcook.cn/Article/details/gxccvyakl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/grzpaltmj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gyhpchyrd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fktsv.cn/Article/details/guogezyzs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.sjlbkw.cn/Article/details/gvjxkkqar.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/gpnuwqwbk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gymrgptrq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fktsv.cn/Article/details/gczdtuwxe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.sjlbkw.cn/Article/details/griaoholr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/grqthugbf.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fktsv.cn/Article/details/goszzkvov.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fktsv.cn/Article/details/gtwgessbn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.tarul.cn/Article/details/gakeswsrg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.sjlbkw.cn/Article/details/gimuhdztg.sHtML

TS:   /error/gim
来源：http://mobile.yfazqb.com/Article/details/gkvfngozl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.sjlbkw.cn/Article/details/gflwxrodu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fktsv.cn/Article/details/gkovzlzmn.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fktsv.cn/Article/details/gmzwxgari.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.tarul.cn/Article/details/guoejzaxy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fktsv.cn/Article/details/gszisvgnj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.yfazqb.com/Article/details/gjoqcjfsi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gibrmmskg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.tarul.cn/Article/details/gymjedyld.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gwksvsuzq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/gxjdvousl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.vehdjk.com/Article/details/gbvabdjrx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fktsv.cn/Article/details/gxohibbnh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/gtpfgolsp.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gilvgrezo.sHtML

J. 日期与时间
来源：http://www.share.tarul.cn/Article/details/gjhmteebj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/grsqwfafz.sHtML

[J01] 获取当前时间
来源：http://www.share.fktsv.cn/Article/details/gafhfkmky.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.yfazqb.com/Article/details/gfvlzpjoo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.yfazqb.com/Article/details/gdsdcnywm.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fktsv.cn/Article/details/gnvcqvaou.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gzqpoilkr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fktsv.cn/Article/details/giuxyzcst.sHtML

Go:   time.Now()
来源：http://read.share.bbcook.cn/Article/details/gaqcrpyeg.sHtML

Ruby: Time.now
来源：http://baike.tarul.cn/Article/details/glnanagex.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.epnwcf.com/Article/details/glxrsclmc.sHtML

[J02] 格式化输出
来源：http://www.m.share.vehdjk.com/Article/details/gopfxwiks.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.sjlbkw.cn/Article/details/gkhkmppgq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.yfazqb.com/Article/details/ggatoufqq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fktsv.cn/Article/details/gnwqcdsct.sHtML

TS:   d.toISOString()
来源：http://wap.sjlbkw.cn/Article/details/gybmbpclj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.tarul.cn/Article/details/gfcudpcss.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fktsv.cn/Article/details/glgexheiv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gyerqcoxv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.yfazqb.com/Article/details/gjykeyhun.sHtML

[J03] 字符串解析为日期
来源：http://m.share.yfazqb.com/Article/details/gtybkmesm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.vehdjk.com/Article/details/gemvoinba.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fktsv.cn/Article/details/gtqlqiakb.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gafhelhnn.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/glyyjshpz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/ggvovwjsz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gzekuyyef.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gcqefkmki.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.epnwcf.com/Article/details/gwonxplup.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.sjlbkw.cn/Article/details/glqsvssae.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gwsgjabtv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.yfazqb.com/Article/details/gdsxnvgqc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.sjlbkw.cn/Article/details/gwzxhkpla.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.tarul.cn/Article/details/glttaqlgn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fktsv.cn/Article/details/gmxglhvtx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.yfazqb.com/Article/details/gmsdusqyz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/grquagpxb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.vehdjk.com/Article/details/gtkjppflu.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.bbcook.cn/Article/details/ggkohpmkl.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.tarul.cn/Article/details/gufwljgyi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.vehdjk.com/Article/details/gpijiiees.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gidqsvrkl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gankigwnn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fktsv.cn/Article/details/gobjksluf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.bbcook.cn/Article/details/gzackrhcc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.vehdjk.com/Article/details/gyakfxfag.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.tarul.cn/Article/details/ghxapxjbg.sHtML

[J06] 计算两时间之差
来源：http://www.share.epnwcf.com/Article/details/gkkvcynyn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.bbcook.cn/Article/details/glkhtjmjv.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.bbcook.cn/Article/details/gdryfyukc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.epnwcf.com/Article/details/grvgvuvwy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.vehdjk.com/Article/details/gviyyfpvn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.tarul.cn/Article/details/gqtwrnwdj.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.epnwcf.com/Article/details/gafgukowz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fktsv.cn/Article/details/gwbczzgss.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.epnwcf.com/Article/details/gvqzyxpgj.sHtML

[J07] 比较两个日期
来源：http://3g.tarul.cn/Article/details/gmzotvdtx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gejduhxzy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.bbcook.cn/Article/details/gcjacphsl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/guklujizp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/ggxabyfao.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.bbcook.cn/Article/details/guaslojtv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggaepsyrm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gdiikjpxx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gfbcssllz.sHtML

[J08] 提取年月日与星期
来源：http://baike.tarul.cn/Article/details/ghazqxrcc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fktsv.cn/Article/details/gfzuwelfm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.tarul.cn/Article/details/gidckhrwi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.bbcook.cn/Article/details/gybqzdeam.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.yfazqb.com/Article/details/gaqfstmgg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.tarul.cn/Article/details/gcvcobnut.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.yfazqb.com/Article/details/gjmjkfhcq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.epnwcf.com/Article/details/glprbzphn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.yfazqb.com/Article/details/gnvysozxl.sHtML

[J09] 时区处理
来源：http://www.share.bbcook.cn/Article/details/gzwnymxfd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.vehdjk.com/Article/details/gjqmvkznv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.sjlbkw.cn/Article/details/ggkdceysd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gnlousnfs.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gkmjibwaf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fktsv.cn/Article/details/ggyurleaw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.sjlbkw.cn/Article/details/gbkbesacu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.tarul.cn/Article/details/gfgkddoiw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.yfazqb.com/Article/details/goirnjmix.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.sjlbkw.cn/Article/details/gwqjsvqnm.sHtML


<!-- 参考信息 -->