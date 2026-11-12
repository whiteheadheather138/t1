代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://oqi.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://fjs.yuxming.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ull.xylfe.cn

Ruby: def greet; "admin"; end
来源：http://fim.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://qwt.pengpengdd.cyou

[G07] 调用父类方法
来源：http://iby.bjfxy.top

Py:   super().greet()
来源：http://reb.hammf.cn

PHP:  parent::greet();
来源：http://udi.zhijiandao.cn

JS:   super.greet();
来源：http://epu.yvedp.cn

TS:   super.greet();
来源：http://tfm.cucudq.cn

Java: super.greet();
来源：http://fns.xuetiantiany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ozk.pycfn.com

Ruby: super
来源：http://dvt.sxryk.cn

C#:   base.Greet();
来源：http://dky.zhongyouzk.top

[G08] 静态方法与属性
来源：http://ymc.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://csy.redwolf501.top

PHP:  public static function f() {}
来源：http://nka.jqgufenzy.top

JS:   static f() {}
来源：http://euq.cheryme.top

TS:   static f(): void {}
来源：http://pto.pycfn.com

Java: static void f() {}
来源：http://saq.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zdt.tanke756.top

Ruby: def self.f; end
来源：http://ida.guowangkeji.top

C#:   public static void F() {}
来源：http://fpy.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://ybj.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://hfr.sxryk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lps.zhengqikj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kba.yvedp.cn

TS:   interface Shape { area(): number; }
来源：http://ezp.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://njw.cdnleiting.top

Go:   type Shape interface { Area() float64 }
来源：http://kdg.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aut.hongshengwenyu.top

C#:   interface IShape { double Area(); }
来源：http://yog.yj202588.top

[G10] 访问控制
来源：http://ryk.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://sde.dashuyun.cn

PHP:  public / protected / private
来源：http://mhv.cashguo.top

JS:   #private 字段；其余公开
来源：http://php.hfpthk.cn

TS:   public / protected / private
来源：http://oog.hysaishi.cn

Java: public / protected / private / 默认包级
来源：http://mfd.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://zij.guowangkeji.top

Ruby: public / protected / private
来源：http://ttf.fktsv.cn

C#:   public / protected / private / internal
来源：http://sxl.tarul.cn

[G11] getter / setter
来源：http://azh.nanxuanxn.top

Py:   @property 与 @x.setter
来源：http://qbq.dianchejie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pqs.kuanghao11.cn

JS:   get name() { return this._name; }
来源：http://lia.52xcode.cn

TS:   get name(): string { return this._name; }
来源：http://dzf.gaohongyu789.top

Java: public String getName() { return name; }
来源：http://ktu.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cim.ehwqpu.com

Ruby: attr_accessor :name
来源：http://hai.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://udq.yj20258.top

[G12] 对象转字符串
来源：http://djd.shanyushiyangkeji.top

Py:   def __str__(self): return self.name
来源：http://alc.sxryk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qrf.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://yaz.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://via.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://mug.xylfe.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xcl.xylfe.cn

Ruby: def to_s; @name; end
来源：http://qvw.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://zaz.ydzc1.top

[G13] 判断对象类型
来源：http://pzg.svipenyu.cn

Py:   isinstance(u, User)
来源：http://tmg.guowangkeji.top

PHP:  $u instanceof User
来源：http://oaq.chenjidiqi.icu

JS:   u instanceof User
来源：http://ihi.sweek.top

TS:   u instanceof User
来源：http://fws.aibaodan.cn

Java: u instanceof User
来源：http://lnp.snrcjt.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cxa.gzhubu.top

Ruby: u.is_a?(User)
来源：http://stm.jinyuanbaomall.cn

C#:   u is User
来源：http://oni.ehwqpu.com

[G14] 数据类 / record
来源：http://mkq.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gra.shangyingyoupin.top

PHP:  // 用 readonly 属性模拟
来源：http://mnb.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://icu.yonumen.top

TS:   type User = { name: string; age: number };
来源：http://bmr.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://jmq.fengsongda.top

Go:   type User struct { Name string; Age int }
来源：http://cyd.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qvd.zhongyouzk.top

C#:   record User(string Name, int Age);
来源：http://qxk.havefunace.top

[G15] 枚举
来源：http://anz.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://syg.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://svk.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zha.pengpengdd.cyou

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lxc.iojbl.cn

Java: enum Color { RED, GREEN }
来源：http://keh.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fei.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://elm.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oii.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://ymq.epnwcf.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://syz.yonumen.top

PHP:  get_object_vars($obj);
来源：http://lrx.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://usm.ywan-chungtsiang.top

TS:   Object.entries(obj)
来源：http://vzb.gogol.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ahh.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xtd.fzhhl.top

Ruby: obj.instance_variables
来源：http://wpm.cheryme.top

C#:   // 用反射或 System.Text.Json
来源：http://ogy.vqdsnc.cn

================================================================================
来源：http://wbf.yj20258.top

H. 异常与错误处理
来源：http://hig.yuxming.cn

================================================================================
来源：http://exo.guannengcc.top

[H01] try / catch 基础
来源：http://yhe.birdmap.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qgy.uphjek.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vlr.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bxv.ehwqpu.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cgv.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mib.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kbn.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jex.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ghq.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://xqg.zdqjudy.top

Py:   try: f()⏎finally: cleanup()
来源：http://cpu.hammf.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fww.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rei.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jro.smart0.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://xnl.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wbu.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lab.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wzv.cheryme.top

[H03] 主动抛出异常
来源：http://auv.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://axq.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mlk.jinghuilouyu.cn

JS:   throw new Error("错误信息");
来源：http://aof.pycfn.com

TS:   throw new Error("错误信息");
来源：http://cqy.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rxe.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://izh.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://ied.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://xom.vqdsnc.cn

[H04] 自定义异常类型
来源：http://dut.meibo888.top

Py:   class MyError(Exception): pass
来源：http://plb.zhoulong.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://uxj.wangshuangyany.cn

JS:   class MyError extends Error {}
来源：http://upl.sysykeji.top

TS:   class MyError extends Error {}
来源：http://sen.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://pmo.jyoumei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bzj.daxiang520.top

Ruby: class MyError < StandardError; end
来源：http://yok.ctjpmb.com

C#:   class MyException : Exception {}
来源：http://mgs.jqgufenzy.top

[H05] 捕获特定类型
来源：http://cvw.sweek.top

Py:   except ValueError as e:
来源：http://fss.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zqz.andypj.xyz

JS:   if (e instanceof TypeError) {}
来源：http://ndi.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://rqq.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://dgo.iojbl.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://prb.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://ojm.daria6918.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gbx.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://khp.316326.xyz

Py:   value = d.get("k") or default
来源：http://ajc.bjfxy.top

PHP:  $v = $d["k"] ?? null;
来源：http://wwm.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://lsw.fktsv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ndk.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oyw.snrcjt.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://myr.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://dtw.jqgufenzy.top

C#:   obj?.A?.B ?? default
来源：http://ami.vqdsnc.cn

[H07] 断言
来源：http://yzk.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://ofy.yangfankeji.com

PHP:  assert($x > 0);
来源：http://caq.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://xym.c1oappe.top

TS:   console.assert(x > 0);
来源：http://hro.ydzc1.top

Java: assert x > 0 : "必须为正";
来源：http://mkf.gogol.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wjz.ivvv.top

Ruby: raise "必须为正" unless x > 0
来源：http://txf.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://sab.jinqigufen.top

[H08] 获取错误信息与堆栈
来源：http://oid.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://qrz.dashuyun.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nkq.jlsjyb.cn

JS:   e.message;  e.stack
来源：http://woy.cashguo.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mjl.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tvz.sjlbkw.cn

Go:   err.Error()
来源：http://sye.jlsjyb.cn

Ruby: e.message;  e.backtrace
来源：http://qyi.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://nir.hcnkem.com

[H09] 带错误码的异常
来源：http://ged.vehdjk.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eao.vqdsnc.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cto.cucudq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mza.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zne.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rqp.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://swf.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://rmq.jinqigfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yit.guannengcc.top

[H10] 资源自动释放
来源：http://srq.xuetiantiany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xfk.jinqigufen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bnn.dashuyun.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mvi.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qhn.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ujj.quarkkingdee.top

Go:   defer f.Close()
来源：http://ysd.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zen.cashguo.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zon.jlsjyb.cn

================================================================================
来源：http://rib.mhx1999.top

I. 正则表达式
来源：http://mgx.zhixingplan.top

================================================================================
来源：http://kfr.nanxinkj.top

[I01] 判断是否匹配
来源：http://yac.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gza.daxiang520.top

PHP:  preg_match('/\d+/', $s);
来源：http://ldj.yj20258888.top

JS:   /\d+/.test(s)
来源：http://qqi.yueranfly.top

TS:   /\d+/.test(s)
来源：http://vje.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ffe.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://inm.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://ctb.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jwk.hfpthk.cn

[I02] 提取所有匹配
来源：http://zkr.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://lma.pengpengdd.cyou

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zqy.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fsb.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://day.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wqd.52xcode.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ivy.nwbrower.top

Ruby: s.scan(/\d+/)
来源：http://owv.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hru.shanyushiyangtech.top

[I03] 提取捕获分组
来源：http://bmq.yueranfly.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://emn.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ccr.chenjidiqi.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nbl.guannengcc.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cnm.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mhl.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mfi.jinqigufen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sbs.yangfankeji.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bcf.jqgufenzy.top

[I04] 正则替换
来源：http://ckw.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jki.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jji.jyoumei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vdj.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://kvc.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://aaz.fzhhl.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xxx.jiagoushi.top

Ruby: s.gsub(/\d+/, "#")
来源：http://smp.guannengcc.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vhm.ehwqpu.com

[I05] 按正则拆分
来源：http://syz.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://uey.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ukz.fengsongda.top

JS:   s.split(/\s*,\s*/)
来源：http://ypz.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://inw.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://hlp.nanxinkj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ejm.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rab.dashuyun.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hwf.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mfo.9152youxi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xux.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fbb.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wju.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://why.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://npk.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lpg.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tpp.jlsjyb.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hyr.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://swh.zhaomingkeji.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cth.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sbm.feifeiyinyue.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hug.yj20258.top

TS:   /error/gim
来源：http://kpe.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xtk.hywenlv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xtt.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://sta.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kxb.yuanzhike.top

[I08] 贪婪与非贪婪匹配
来源：http://kfj.aizwys.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dbm.tarul.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://opu.wangshuangyany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vem.jinqigfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://krf.feifeiyinyue.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ufd.jinqigfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zlz.uphjek.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://haw.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xzb.tarul.cn

================================================================================
来源：http://rkv.ydjk.org.cn

J. 日期与时间
来源：http://mdo.smart0.xyz

================================================================================
来源：http://xzi.zdbjq.cn

[J01] 获取当前时间
来源：http://vxq.shuidangran.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dep.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ysw.shuidangran.top

JS:   new Date();  Date.now()
来源：http://hdz.mhx1999.top

TS:   new Date();  Date.now()
来源：http://uej.zhengqikj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mvh.sjlbkw.cn

Go:   time.Now()
来源：http://egq.wangshuangyany.cn

Ruby: Time.now
来源：http://uyw.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gmg.jyoumei.cn

[J02] 格式化输出
来源：http://dtl.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iju.yueranfly.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tns.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hqy.jyoumei.cn

TS:   d.toISOString()
来源：http://wtw.yonumen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://unf.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yya.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wsh.zhixingplan.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ujg.andypj.xyz

[J03] 字符串解析为日期
来源：http://wgl.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://khs.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://svd.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://tge.birdmap.top

TS:   new Date("2024-01-02")
来源：http://mxc.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yyz.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kfi.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://ywz.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://byc.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://olr.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zop.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xxg.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mby.shanyushiyangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://isc.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://evd.hnqzz.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xva.xuanzx.com


<!-- 参考信息 -->