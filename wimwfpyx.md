代发 wailian999

PHP:  public static function f() {}
来源：http://duo.jianghu66.top

JS:   static f() {}
来源：http://qfy.tarul.cn

TS:   static f(): void {}
来源：http://xjr.yangfankeji.com

Java: static void f() {}
来源：http://sag.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xcd.xuanzx.com

Ruby: def self.f; end
来源：http://ipi.xuetiantiany.cn

C#:   public static void F() {}
来源：http://wua.pycfn.com

[G09] 接口 / 抽象类
来源：http://opw.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://qkg.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uax.cashguo.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mzo.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://ixg.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://lkm.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://ojv.316326.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bne.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://vyx.vqdsnc.cn

[G10] 访问控制
来源：http://agu.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://pea.xylfe.cn

PHP:  public / protected / private
来源：http://mht.sweek.top

JS:   #private 字段；其余公开
来源：http://tdz.ctjpmb.com

TS:   public / protected / private
来源：http://ywm.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://jje.daria6918.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dfm.wangdashe.top

Ruby: public / protected / private
来源：http://qsb.svipenyu.cn

C#:   public / protected / private / internal
来源：http://cje.52xcode.cn

[G11] getter / setter
来源：http://cwb.shanyushiyangkeji.top

Py:   @property 与 @x.setter
来源：http://znv.tian-w.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kxn.hammf.cn

JS:   get name() { return this._name; }
来源：http://sfm.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://xlm.daria6918.cn

Java: public String getName() { return name; }
来源：http://jmi.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://oog.yueranfly.top

Ruby: attr_accessor :name
来源：http://ijk.fehbvm.com

C#:   public string Name { get; set; }
来源：http://lgq.guowangkeji.top

[G12] 对象转字符串
来源：http://ywa.havefunace.top

Py:   def __str__(self): return self.name
来源：http://dtm.ehwqpu.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://kwj.0kj1m.cn

JS:   toString() { return this.name; }
来源：http://djc.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://xgg.shzxlz.cn

Java: @Override public String toString() { return name; }
来源：http://bir.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://iri.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://rvp.hcnkem.com

C#:   public override string ToString() => Name;
来源：http://lrl.yvedp.cn

[G13] 判断对象类型
来源：http://rqj.sysykeji.top

Py:   isinstance(u, User)
来源：http://rvg.epnwcf.com

PHP:  $u instanceof User
来源：http://xzx.hongshengwenyu.top

JS:   u instanceof User
来源：http://qtv.guowangkeji.top

TS:   u instanceof User
来源：http://fsi.sufxvd.cn

Java: u instanceof User
来源：http://syg.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://zli.fktsv.cn

Ruby: u.is_a?(User)
来源：http://uno.zhiwuduotai.top

C#:   u is User
来源：http://jvc.jqgufenzy.top

[G14] 数据类 / record
来源：http://bdb.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xqb.sjlbkw.cn

PHP:  // 用 readonly 属性模拟
来源：http://yjx.xylfe.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yvp.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://ybf.yongpay.top

Java: record User(String name, int age) {}
来源：http://uir.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://jol.hongshengwenyu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jie.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://ayt.cheryme.top

[G15] 枚举
来源：http://xap.52xcode.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sxv.zhiwuduotai.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://foz.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://isa.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://owu.316326.xyz

Java: enum Color { RED, GREEN }
来源：http://dvn.zhongyouzk.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qug.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://wwb.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://knv.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://sqt.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xfw.jqgufenzy.top

PHP:  get_object_vars($obj);
来源：http://bwg.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://kov.ydzc1.top

TS:   Object.entries(obj)
来源：http://hln.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oqd.yangfankeji.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://evn.52xcode.cn

Ruby: obj.instance_variables
来源：http://mue.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://tgz.jlsjyb.cn

================================================================================
来源：http://bnz.gzhubu.top

H. 异常与错误处理
来源：http://vlt.jyoumei.cn

================================================================================
来源：http://clr.zhiwuduotai.top

[H01] try / catch 基础
来源：http://soi.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://okp.cucudq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qni.hywenlv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iuk.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iwb.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fta.jinyuanbaomall.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zvy.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ixc.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ebv.epnwcf.com

[H02] finally / ensure 收尾
来源：http://qqu.chenlongwang.top

Py:   try: f()⏎finally: cleanup()
来源：http://eld.zhaomingkeji.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://ggw.pengpengdd.cyou

JS:   try { f(); } finally { cleanup(); }
来源：http://idf.sweek.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zum.guannengcc.top

Java: try { f(); } finally { cleanup(); }
来源：http://qvs.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qkq.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://mfv.smart0.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://oxv.zycfv.cn

[H03] 主动抛出异常
来源：http://kxd.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://cyl.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yqg.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://bdh.xuanzx.com

TS:   throw new Error("错误信息");
来源：http://toj.epnwcf.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://wrk.hysaishi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lns.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hje.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://law.tian-w.cn

[H04] 自定义异常类型
来源：http://vtk.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://fab.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://unm.jinqigufen.top

JS:   class MyError extends Error {}
来源：http://pau.jyoumei.cn

TS:   class MyError extends Error {}
来源：http://hcz.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://gbw.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nfm.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://aor.shangyingyoupin.top

C#:   class MyException : Exception {}
来源：http://hbk.ivvv.top

[H05] 捕获特定类型
来源：http://fka.bbcook.cn

Py:   except ValueError as e:
来源：http://cbj.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ipz.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://vhu.cucudq.cn

TS:   if (e instanceof TypeError) {}
来源：http://mae.pycfn.com

Java: catch (IOException | SQLException e) {}
来源：http://vcu.fehbvm.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ftl.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://dqu.yueranfly.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oqe.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://cqr.gogol.net.cn

Py:   value = d.get("k") or default
来源：http://txx.pengpengdd.cyou

PHP:  $v = $d["k"] ?? null;
来源：http://hog.sweek.top

JS:   obj?.a?.b;  d ?? default
来源：http://efl.cdnleiting.top

TS:   obj?.a?.b;  d ?? default
来源：http://reu.ydjk.org.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ktm.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hen.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://hpe.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://swb.hnxiangtu.top

[H07] 断言
来源：http://lpc.wangdashe.top

Py:   assert x > 0, "必须为正"
来源：http://lqt.fanxiaobao.xyz

PHP:  assert($x > 0);
来源：http://msv.yfazqb.com

JS:   console.assert(x > 0);
来源：http://hjf.sxryk.cn

TS:   console.assert(x > 0);
来源：http://jeh.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://jhb.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://esa.fehbvm.com

Ruby: raise "必须为正" unless x > 0
来源：http://lcd.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://lzm.birdmap.top

[H08] 获取错误信息与堆栈
来源：http://rbx.tianlin.xyz

Py:   str(e);  traceback.format_exc()
来源：http://yre.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jzu.havefunace.top

JS:   e.message;  e.stack
来源：http://kzf.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rsg.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ksy.pengpengdd.cyou

Go:   err.Error()
来源：http://ccb.meibo888.top

Ruby: e.message;  e.backtrace
来源：http://rhc.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://ura.aizwys.cn

[H09] 带错误码的异常
来源：http://opo.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fxz.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ydx.hnqzz.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hes.nwbrower.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nzw.hywenlv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uyr.hnxiangtu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rst.xuetiantiany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zag.cqqwz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hrk.guannengcc.top

[H10] 资源自动释放
来源：http://ckm.nanxuanxn.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kst.yuanzhike.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vix.gotoacloud.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ybz.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://okz.fzhhl.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://img.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://dhi.yongpay.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rym.yongpay.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dbn.zhaomingkeji.xyz

================================================================================
来源：http://sik.wangshuangyany.cn

I. 正则表达式
来源：http://ljp.vqdsnc.cn

================================================================================
来源：http://hqs.gogol.net.cn

[I01] 判断是否匹配
来源：http://lkq.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mbf.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://csd.ydzc1.top

JS:   /\d+/.test(s)
来源：http://wdl.yongpay.top

TS:   /\d+/.test(s)
来源：http://voq.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://shu.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lwb.dashuyun.cn

Ruby: s.match?(/\d+/)
来源：http://bbm.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pwu.zhijiandao.cn

[I02] 提取所有匹配
来源：http://tzw.vehdjk.com

Py:   re.findall(r"\d+", s)
来源：http://rua.jlsjyb.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kza.epnwcf.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fnd.zhixingplan.top

TS:   s.match(/\d+/g)
来源：http://vix.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://noa.jianghu66.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sgm.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://nbx.tian-w.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tzi.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://fvg.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ukw.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vvz.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dya.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ylo.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vrs.jinyuanbaomall.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://meg.cucudq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cvz.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ipy.cdnleiting.top

[I04] 正则替换
来源：http://zab.chenjidiqi.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://ajc.vehdjk.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qne.jinyuanbaomall.cn

JS:   s.replace(/\d+/g, "#")
来源：http://inz.svipenyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kgo.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://jjw.hnqzz.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xqd.hongshengwenyu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fbm.hcnkem.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://evu.ybcxt.top

[I05] 按正则拆分
来源：http://pwc.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xcj.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wip.ivvv.top

JS:   s.split(/\s*,\s*/)
来源：http://gxe.shangyingyoupin.top

TS:   s.split(/\s*,\s*/)
来源：http://rki.jinyuanbaomall.cn

Java: s.split("\\s*,\\s*")
来源：http://kde.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sll.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://zfb.52xcode.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://frj.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fam.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bsj.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://skx.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cqa.ybcxt.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zwi.jinyuanbaomall.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eds.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uon.zhijiandao.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wuh.yfazqb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yym.hysaishi.cn

[I07] 忽略大小写与多行模式
来源：http://mku.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jcp.shangyingyoupin.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://auo.zhongyouzk.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qlu.yuanzhike.top

TS:   /error/gim
来源：http://muw.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oxr.yvedp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sws.zycfv.cn

Ruby: s.scan(/error/i)
来源：http://nmd.sjlbkw.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://odg.svipenyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://bnf.yuxming.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yit.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pfm.snrcjt.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jbe.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hfy.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rca.jiagoushi.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tag.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tik.0kj1m.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lyb.hammf.cn

================================================================================
来源：http://uxv.zdqjudy.top

J. 日期与时间
来源：http://ojv.xuanzx.com

================================================================================
来源：http://mmb.gotoacloud.top

[J01] 获取当前时间
来源：http://zyz.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sgp.tarul.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fte.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://ogx.guannengcc.top

TS:   new Date();  Date.now()
来源：http://kds.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tsw.hywenlv.cn

Go:   time.Now()
来源：http://izn.tianlin.xyz

Ruby: Time.now
来源：http://fnn.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jdd.zdqjudy.top

[J02] 格式化输出
来源：http://wuk.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bpq.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tot.shanyushiyangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://syr.cheryme.top

TS:   d.toISOString()
来源：http://cwv.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qmj.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yik.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yzw.yj202588.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zki.nanxinkj.top

[J03] 字符串解析为日期
来源：http://fjy.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fgn.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pox.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://msd.birdmap.top

TS:   new Date("2024-01-02")
来源：http://mxj.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://jns.vqdsnc.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wip.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://rli.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lgu.bbcook.cn

[J04] 时间戳与日期互转
来源：http://esk.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tqq.ctjpmb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fpp.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lqx.meibo888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tta.hywenlv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nsn.ppjwa.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pug.yj20258888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fss.fktsv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pde.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://dya.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://tjv.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://xnf.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ean.sxryk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rbp.nanxinkj.top

Java: LocalDate.now().plusDays(7)
来源：http://cux.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gem.dashuyun.cn

Ruby: Time.now + 7 * 86400
来源：http://xyp.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://dss.yj202588.top

[J06] 计算两时间之差
来源：http://nxp.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://ihy.ybcxt.top

PHP:  $end->diff($start)->days;
来源：http://ubv.yuxming.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qzg.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nid.shuidangran.top


<!-- 参考信息 -->