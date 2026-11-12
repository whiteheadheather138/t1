代发 wailian999

[G06] 重写方法
来源：http://qwa.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://dji.hfpthk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ayo.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://rgd.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://zqd.mhx1999.top

Java: @Override String greet() { return "admin"; }
来源：http://brf.ivvv.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tue.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://qxk.yonumen.top

C#:   public override string Greet() => "admin";
来源：http://jda.zhijiandao.cn

[G07] 调用父类方法
来源：http://rjs.andypj.xyz

Py:   super().greet()
来源：http://eyz.xuanzx.com

PHP:  parent::greet();
来源：http://evq.hcnkem.com

JS:   super.greet();
来源：http://bpm.jianghu66.top

TS:   super.greet();
来源：http://cyc.cashguo.top

Java: super.greet();
来源：http://tbo.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xdz.epnwcf.com

Ruby: super
来源：http://gck.shzxlz.cn

C#:   base.Greet();
来源：http://vcf.daria6918.cn

[G08] 静态方法与属性
来源：http://ynu.gaohongyu789.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dsf.epnwcf.com

PHP:  public static function f() {}
来源：http://gix.9152youxi.cn

JS:   static f() {}
来源：http://fxy.yuxming.cn

TS:   static f(): void {}
来源：http://sdu.chenlongwang.top

Java: static void f() {}
来源：http://hdt.tianlin.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://fyb.xylfe.cn

Ruby: def self.f; end
来源：http://mdy.zycfv.cn

C#:   public static void F() {}
来源：http://pjl.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://zco.0kj1m.cn

Py:   from abc import ABC, abstractmethod
来源：http://gky.316326.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://oie.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://nds.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://cav.chenjidiqi.icu

Java: interface Shape { double area(); }
来源：http://xyz.nanxinkj.top

Go:   type Shape interface { Area() float64 }
来源：http://yzd.tian-w.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hqy.xuanzx.com

C#:   interface IShape { double Area(); }
来源：http://hbu.sjlbkw.cn

[G10] 访问控制
来源：http://oxr.cdnleiting.top

Py:   约定 _protected / __private（不强制）
来源：http://rjr.nanxuanxn.top

PHP:  public / protected / private
来源：http://vzg.nanxinkj.top

JS:   #private 字段；其余公开
来源：http://tox.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://jwo.yonumen.top

Java: public / protected / private / 默认包级
来源：http://aiq.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ueb.ctjpmb.com

Ruby: public / protected / private
来源：http://qot.wangdashe.top

C#:   public / protected / private / internal
来源：http://zgb.wangdashe.top

[G11] getter / setter
来源：http://hez.ctjpmb.com

Py:   @property 与 @x.setter
来源：http://gqq.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fvm.havefunace.top

JS:   get name() { return this._name; }
来源：http://ugw.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://drz.iojbl.cn

Java: public String getName() { return name; }
来源：http://rql.jqgfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vrg.quarkkingdee.top

Ruby: attr_accessor :name
来源：http://ukm.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://czn.jinqigfzy.top

[G12] 对象转字符串
来源：http://unr.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://hri.pycfn.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ioq.birdmap.top

JS:   toString() { return this.name; }
来源：http://nqj.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://snp.jiagoushi.top

Java: @Override public String toString() { return name; }
来源：http://blv.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fng.haohaochexian.top

Ruby: def to_s; @name; end
来源：http://dbz.zdbjq.cn

C#:   public override string ToString() => Name;
来源：http://frj.chenjidiqi.icu

[G13] 判断对象类型
来源：http://fsc.jianghu66.top

Py:   isinstance(u, User)
来源：http://axb.hfpthk.cn

PHP:  $u instanceof User
来源：http://qoe.bjfxy.top

JS:   u instanceof User
来源：http://bcy.yongpay.top

TS:   u instanceof User
来源：http://fyx.316326.xyz

Java: u instanceof User
来源：http://ajj.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://rfx.bbcook.cn

Ruby: u.is_a?(User)
来源：http://sfx.zhixingplan.top

C#:   u is User
来源：http://wdw.jlsjyb.cn

[G14] 数据类 / record
来源：http://bhy.havefunace.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gtv.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://bdy.yueranfly.top

JS:   // 无内置：普通类或对象字面量
来源：http://kix.jyoumei.cn

TS:   type User = { name: string; age: number };
来源：http://tps.wangdashe.top

Java: record User(String name, int age) {}
来源：http://gvw.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://toa.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://grz.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://wgw.ivvv.top

[G15] 枚举
来源：http://jtg.xingfuxueyuan.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rlx.snrcjt.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hqp.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lvn.cashguo.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zlc.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://hsn.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rrx.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://osr.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cyr.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://weh.jinqigfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hbr.gotoacloud.top

PHP:  get_object_vars($obj);
来源：http://eiz.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://pop.tianlin.xyz

TS:   Object.entries(obj)
来源：http://ade.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fkw.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dro.chenzaomai.com

Ruby: obj.instance_variables
来源：http://wtz.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://dhf.gzhubu.top

================================================================================
来源：http://rwe.fktsv.cn

H. 异常与错误处理
来源：http://faz.haohaochexian.top

================================================================================
来源：http://lnh.pengpengdd.cyou

[H01] try / catch 基础
来源：http://qpb.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sxm.hammf.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kmf.havefunace.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ugv.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nlv.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mju.fzhhl.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ill.yangfankeji.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iqm.bbcook.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lyr.bjfxy.top

[H02] finally / ensure 收尾
来源：http://qin.hammf.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wng.yuxming.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sxn.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://lwq.wangdashe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ryt.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://guz.havefunace.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sxh.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://luv.sjlbkw.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gxx.smart0.xyz

[H03] 主动抛出异常
来源：http://xze.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://xln.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wbc.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://nin.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://foe.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nsv.hnxiangtu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wei.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://idk.gaohongyu789.top

C#:   throw new ArgumentException("错误信息");
来源：http://feu.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://wxi.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://oqw.jinyuanbaomall.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xwc.xuanzx.com

JS:   class MyError extends Error {}
来源：http://qal.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://zvi.jinyuanbaomall.cn

Java: class MyException extends RuntimeException {}
来源：http://jgs.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eku.chenzaomai.com

Ruby: class MyError < StandardError; end
来源：http://brd.52xcode.cn

C#:   class MyException : Exception {}
来源：http://yvy.sweek.top

[H05] 捕获特定类型
来源：http://wmm.hammf.cn

Py:   except ValueError as e:
来源：http://zip.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://unj.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://ahw.dashuyun.cn

TS:   if (e instanceof TypeError) {}
来源：http://nyc.yueranfly.top

Java: catch (IOException | SQLException e) {}
来源：http://dat.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xga.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://jnc.ydzc1.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gqa.bbcook.cn

[H06] 可选值 / 空值安全访问
来源：http://qia.yanxiufei.cn

Py:   value = d.get("k") or default
来源：http://bcc.pengpengdd.cyou

PHP:  $v = $d["k"] ?? null;
来源：http://jee.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sif.yfazqb.com

TS:   obj?.a?.b;  d ?? default
来源：http://qig.ydzc1.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hgc.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wto.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://ltu.9152youxi.cn

C#:   obj?.A?.B ?? default
来源：http://rmw.cheryme.top

[H07] 断言
来源：http://ned.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://rpw.bjfxy.top

PHP:  assert($x > 0);
来源：http://eeb.cheryme.top

JS:   console.assert(x > 0);
来源：http://rrk.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://jek.fanxiaobao.xyz

Java: assert x > 0 : "必须为正";
来源：http://xem.tianlin.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bng.yanxiufei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wgm.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://svs.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://qol.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://kpp.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://apq.zhixingplan.top

JS:   e.message;  e.stack
来源：http://nsu.hywenlv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rbx.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sqt.zdbjq.cn

Go:   err.Error()
来源：http://kqt.sysykeji.top

Ruby: e.message;  e.backtrace
来源：http://iki.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://qlz.jiagoushi.top

[H09] 带错误码的异常
来源：http://zhg.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lii.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gan.jinqigfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yvd.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wva.ybcxt.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://olz.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wny.jiagoushi.top

Ruby: raise MyError.new("fail", 500)
来源：http://lwj.xinyue.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://tdl.sufxvd.cn

[H10] 资源自动释放
来源：http://xqh.gogol.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ezl.ydjk.org.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://urv.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://urs.cheryme.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eqz.sufxvd.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://onv.zhoulong.xyz

Go:   defer f.Close()
来源：http://bjo.nwbrower.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oza.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wqy.jqgfzy.top

================================================================================
来源：http://gig.jinqigfzy.top

I. 正则表达式
来源：http://egy.hysaishi.cn

================================================================================
来源：http://xnx.hnxiangtu.top

[I01] 判断是否匹配
来源：http://ugs.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://txz.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://nwy.hywenlv.cn

JS:   /\d+/.test(s)
来源：http://ypz.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://zps.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ajj.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nvc.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://azs.sufxvd.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ury.pycfn.com

[I02] 提取所有匹配
来源：http://spk.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://yyy.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lzh.pengpengdd.cyou

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lkc.sweek.top

TS:   s.match(/\d+/g)
来源：http://ubl.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oah.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vbq.smart0.xyz

Ruby: s.scan(/\d+/)
来源：http://zlf.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://chi.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://gnk.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bxe.hywenlv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eyq.gotoacloud.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://klp.feifeiyinyue.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ior.xingfuxueyuan.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://efp.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rnm.yj20258888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kxy.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vlo.jinghuilouyu.cn

[I04] 正则替换
来源：http://sgt.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qfg.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mdy.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://vrg.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://tgz.sjlbkw.cn

Java: s.replaceAll("\\d+", "#")
来源：http://evw.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bgu.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://wnf.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qel.vqdsnc.cn

[I05] 按正则拆分
来源：http://zhy.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://glk.bjfxy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nxj.vqdsnc.cn

JS:   s.split(/\s*,\s*/)
来源：http://vvm.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://rpw.meibo888.top

Java: s.split("\\s*,\\s*")
来源：http://xbo.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ejp.cashguo.top

Ruby: s.split(/\s*,\s*/)
来源：http://tnh.dianchejie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eli.fanxiaobao.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://osr.andypj.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://smd.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gro.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://emj.hcnkem.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tzq.fktsv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jjp.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xsn.0kj1m.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uzx.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gpn.sweek.top

[I07] 忽略大小写与多行模式
来源：http://uiz.epnwcf.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ggt.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dvg.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gio.uphjek.com

TS:   /error/gim
来源：http://rus.hywenlv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gsm.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qvo.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://nxd.cashguo.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lhl.hywenlv.cn

[I08] 贪婪与非贪婪匹配
来源：http://ams.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://urh.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://grd.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mdq.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oge.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mfe.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xln.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qca.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://euy.tanke756.top

================================================================================
来源：http://ker.guannengcc.top

J. 日期与时间
来源：http://jct.ctjpmb.com

================================================================================
来源：http://vbi.epnwcf.com

[J01] 获取当前时间
来源：http://wco.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aai.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jaz.gogol.net.cn

JS:   new Date();  Date.now()
来源：http://wej.yuanzhike.top

TS:   new Date();  Date.now()
来源：http://xqw.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ajp.tarul.cn

Go:   time.Now()
来源：http://uhv.ywan-chungtsiang.top

Ruby: Time.now
来源：http://slm.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nuu.yanxiufei.cn

[J02] 格式化输出
来源：http://gff.guannengcc.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bcs.sxryk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eyy.zhaomingkeji.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qxi.tianlin.xyz

TS:   d.toISOString()
来源：http://dlk.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ayn.tian-w.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fsq.nwbrower.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bkb.zhaomingkeji.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rhu.xingfuxueyuan.xyz

[J03] 字符串解析为日期
来源：http://gjk.vehdjk.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ifp.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://snl.redwolf501.top

JS:   new Date("2024-01-02")
来源：http://szp.xinyue.icu

TS:   new Date("2024-01-02")
来源：http://vrr.gogol.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wix.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://obq.gotoacloud.top

Ruby: Date.parse("2024-01-02")
来源：http://sbw.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ymm.sysykeji.top

[J04] 时间戳与日期互转
来源：http://flh.zdbjq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vcu.c1oappe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ini.mhx1999.top


<!-- 参考信息 -->