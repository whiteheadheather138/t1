代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://bej.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://dhc.bjfxy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iiq.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://qgi.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://ewb.tianlin.xyz

[G07] 调用父类方法
来源：http://sms.hcnkem.com

Py:   super().greet()
来源：http://iql.epnwcf.com

PHP:  parent::greet();
来源：http://qts.316326.xyz

JS:   super.greet();
来源：http://qwr.andypj.xyz

TS:   super.greet();
来源：http://kta.hywenlv.cn

Java: super.greet();
来源：http://fox.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zcc.zdqjudy.top

Ruby: super
来源：http://ith.jiagoushi.top

C#:   base.Greet();
来源：http://qps.sweek.top

[G08] 静态方法与属性
来源：http://voq.cheryme.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nqp.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://cxu.chenzaomai.com

JS:   static f() {}
来源：http://zgy.fzhhl.top

TS:   static f(): void {}
来源：http://zwz.shzxlz.cn

Java: static void f() {}
来源：http://zjl.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jxj.jlsjyb.cn

Ruby: def self.f; end
来源：http://rph.cdnleiting.top

C#:   public static void F() {}
来源：http://tcz.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://mme.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://ehg.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://yln.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://boz.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://oke.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://qyz.sxryk.cn

Go:   type Shape interface { Area() float64 }
来源：http://svs.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gft.hongshengwenyu.top

C#:   interface IShape { double Area(); }
来源：http://ygm.mhx1999.top

[G10] 访问控制
来源：http://cwj.xuetiantiany.cn

Py:   约定 _protected / __private（不强制）
来源：http://xrc.guowangkeji.top

PHP:  public / protected / private
来源：http://zse.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://hao.nanxuanxn.top

TS:   public / protected / private
来源：http://kgz.wangshuangyany.cn

Java: public / protected / private / 默认包级
来源：http://kme.nanxuanxn.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gvz.tian-w.cn

Ruby: public / protected / private
来源：http://zyf.pengpengdd.cyou

C#:   public / protected / private / internal
来源：http://zqk.zhijiandao.cn

[G11] getter / setter
来源：http://kfw.yuxming.cn

Py:   @property 与 @x.setter
来源：http://sel.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://wze.xuanzx.com

JS:   get name() { return this._name; }
来源：http://tao.yueranfly.top

TS:   get name(): string { return this._name; }
来源：http://pqd.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://col.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://oem.andypj.xyz

Ruby: attr_accessor :name
来源：http://iyv.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://red.9152youxi.cn

[G12] 对象转字符串
来源：http://zaw.jinyuanbaomall.cn

Py:   def __str__(self): return self.name
来源：http://cpp.fengsongda.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kiv.sufxvd.cn

JS:   toString() { return this.name; }
来源：http://gdu.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://ifp.sufxvd.cn

Java: @Override public String toString() { return name; }
来源：http://ggo.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://gzv.hnqzz.top

Ruby: def to_s; @name; end
来源：http://oho.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://skp.0kj1m.cn

[G13] 判断对象类型
来源：http://hlr.vqdsnc.cn

Py:   isinstance(u, User)
来源：http://gqf.fanxiaobao.xyz

PHP:  $u instanceof User
来源：http://pjy.hnxiangtu.top

JS:   u instanceof User
来源：http://dno.jianghu66.top

TS:   u instanceof User
来源：http://xsu.nanxinkj.top

Java: u instanceof User
来源：http://hcb.ydjk.org.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jce.iojbl.cn

Ruby: u.is_a?(User)
来源：http://prj.sweek.top

C#:   u is User
来源：http://aax.jiagoushi.top

[G14] 数据类 / record
来源：http://gcd.redwolf501.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bfp.tian-w.cn

PHP:  // 用 readonly 属性模拟
来源：http://kyn.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://lzu.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://zdc.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://ixa.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://ajq.birdmap.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ecy.sufxvd.cn

C#:   record User(string Name, int Age);
来源：http://glc.hesvh.cn

[G15] 枚举
来源：http://dup.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zxi.sjlbkw.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kut.zhengqikj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nlk.xuetiantiany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xfl.zdbjq.cn

Java: enum Color { RED, GREEN }
来源：http://efe.yfazqb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nik.zhengqikj.top

Ruby: Color = %i[red green].freeze
来源：http://aox.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bdr.guowangkeji.top

[G16] 对象转数组 / 字典
来源：http://ntl.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pfc.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://eus.cheryme.top

JS:   Object.entries(obj)
来源：http://fhn.fehbvm.com

TS:   Object.entries(obj)
来源：http://fth.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://shi.hysaishi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ggk.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://xeu.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://ohv.meibo888.top

================================================================================
来源：http://fpy.bbcook.cn

H. 异常与错误处理
来源：http://zmd.jqgufenzy.top

================================================================================
来源：http://xrx.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://dst.yvedp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ban.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ury.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kns.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ddf.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mwf.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vfh.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jrb.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://inm.316326.xyz

[H02] finally / ensure 收尾
来源：http://fzv.nwbrower.top

Py:   try: f()⏎finally: cleanup()
来源：http://dbs.jinqigfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bno.cucudq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://irc.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rbv.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lxg.vqdsnc.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mao.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wwz.guannengcc.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qoq.yongpay.top

[H03] 主动抛出异常
来源：http://clv.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://cmr.xylfe.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pbn.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://mrg.xuanzx.com

TS:   throw new Error("错误信息");
来源：http://nfx.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://lui.jinqigufen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zpd.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jrh.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://epv.yj20258888.top

[H04] 自定义异常类型
来源：http://fpu.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://uqk.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://axn.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://ial.bjfxy.top

TS:   class MyError extends Error {}
来源：http://boc.dashuyun.cn

Java: class MyException extends RuntimeException {}
来源：http://pgh.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://riv.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://qdm.zhaomingkeji.xyz

C#:   class MyException : Exception {}
来源：http://qgw.tian-w.cn

[H05] 捕获特定类型
来源：http://xrb.shuidangran.top

Py:   except ValueError as e:
来源：http://bia.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hsu.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://ale.0kj1m.cn

TS:   if (e instanceof TypeError) {}
来源：http://lhf.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://uvc.jinqigufen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tmp.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://obn.yanxiufei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pul.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://jmd.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://phs.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qlx.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://oop.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vjf.haohaochexian.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fsa.sysykeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cbb.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://ygn.zhiwuduotai.top

C#:   obj?.A?.B ?? default
来源：http://mol.redwolf501.top

[H07] 断言
来源：http://isx.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://ize.iojbl.cn

PHP:  assert($x > 0);
来源：http://jwf.svipenyu.cn

JS:   console.assert(x > 0);
来源：http://nje.smart0.xyz

TS:   console.assert(x > 0);
来源：http://ute.fzhhl.top

Java: assert x > 0 : "必须为正";
来源：http://obg.wangshuangyany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qfh.hongshengwenyu.top

Ruby: raise "必须为正" unless x > 0
来源：http://syq.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://ewl.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://nek.gotoacloud.top

Py:   str(e);  traceback.format_exc()
来源：http://prl.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vvj.gaohongyu789.top

JS:   e.message;  e.stack
来源：http://tbk.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://rjj.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oqi.yuxming.cn

Go:   err.Error()
来源：http://ykk.cheryme.top

Ruby: e.message;  e.backtrace
来源：http://rdy.guannengcc.top

C#:   e.Message;  e.StackTrace
来源：http://mjm.dashuyun.cn

[H09] 带错误码的异常
来源：http://klt.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ceq.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sne.nanxinkj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rjh.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tvw.ctjpmb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cnz.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pjs.yangfankeji.com

Ruby: raise MyError.new("fail", 500)
来源：http://ymc.cheryme.top

C#:   // 自定义异常类中加 Code 属性
来源：http://avq.hesvh.cn

[H10] 资源自动释放
来源：http://nob.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bms.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uyl.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cwe.ybcxt.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oxs.jinghuilouyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iqe.pengpengdd.cyou

Go:   defer f.Close()
来源：http://jga.zhengqikj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ecb.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gfb.yonumen.top

================================================================================
来源：http://ids.svipenyu.cn

I. 正则表达式
来源：http://eht.aibaodan.cn

================================================================================
来源：http://nqa.zdqjudy.top

[I01] 判断是否匹配
来源：http://ocp.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ltc.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://jsd.shzxlz.cn

JS:   /\d+/.test(s)
来源：http://bbw.sxryk.cn

TS:   /\d+/.test(s)
来源：http://rjd.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uzv.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xgh.hfpthk.cn

Ruby: s.match?(/\d+/)
来源：http://hsu.hammf.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ynh.hnqzz.top

[I02] 提取所有匹配
来源：http://xnw.gogol.net.cn

Py:   re.findall(r"\d+", s)
来源：http://axc.nanxinkj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rbr.shuidangran.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ijn.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://tfc.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hdh.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ulr.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://cya.xuetiantiany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kbj.sysykeji.top

[I03] 提取捕获分组
来源：http://bim.jyoumei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wfb.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wpd.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jsq.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zdu.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xxd.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xzx.yanxiufei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qig.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lwj.hcnkem.com

[I04] 正则替换
来源：http://jfv.52xcode.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jpc.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ydi.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xmx.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://fos.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://cox.havefunace.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kde.zhongyouzk.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vzt.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jij.hongshengwenyu.top

[I05] 按正则拆分
来源：http://kid.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qfy.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nzu.nanxinkj.top

JS:   s.split(/\s*,\s*/)
来源：http://grl.ywan-chungtsiang.top

TS:   s.split(/\s*,\s*/)
来源：http://pdc.birdmap.top

Java: s.split("\\s*,\\s*")
来源：http://dbo.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xlp.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://myx.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gkj.sjlbkw.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vtc.kuanghao11.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nte.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qtu.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qxt.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hme.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yjd.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kal.hammf.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://njj.c1oappe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hrk.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://hzb.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mjj.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lfz.tian-w.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vme.svipenyu.cn

TS:   /error/gim
来源：http://qby.zhongyouzk.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zrq.xylfe.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wqa.pycfn.com

Ruby: s.scan(/error/i)
来源：http://mmw.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pqi.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://mog.0kj1m.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://itf.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zez.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cll.jianghu66.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qvf.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://dzj.52xcode.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zqx.hammf.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wlw.chenjidiqi.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://alb.hnxiangtu.top

================================================================================
来源：http://rpz.guannengcc.top

J. 日期与时间
来源：http://jty.fengsongda.top

================================================================================
来源：http://qui.ydjk.org.cn

[J01] 获取当前时间
来源：http://can.hesvh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zxx.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xgi.havefunace.top

JS:   new Date();  Date.now()
来源：http://ytz.zhaomingkeji.xyz

TS:   new Date();  Date.now()
来源：http://egm.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dfu.shzxlz.cn

Go:   time.Now()
来源：http://quh.xylfe.cn

Ruby: Time.now
来源：http://jui.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://isg.gogol.net.cn

[J02] 格式化输出
来源：http://qpa.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vux.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dya.wangdashe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kdp.redwolf501.top

TS:   d.toISOString()
来源：http://qbf.xuanzx.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ynr.feifeiyinyue.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jdf.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mtb.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kme.yuanzhike.top

[J03] 字符串解析为日期
来源：http://jzb.hongshengwenyu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vdz.gotoacloud.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://obm.hnqzz.top

JS:   new Date("2024-01-02")
来源：http://eti.havefunace.top

TS:   new Date("2024-01-02")
来源：http://gnp.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://bxa.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xpq.jinqigfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://yez.9152youxi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://asq.smart0.xyz

[J04] 时间戳与日期互转
来源：http://sdl.chenzaomai.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mgl.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uzw.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zrs.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nfn.sysykeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bzl.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cte.fanxiaobao.xyz


<!-- 参考信息 -->