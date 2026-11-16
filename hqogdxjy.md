代发 wailian999

[G06] 重写方法
来源：http://qrp.pycfn.com

Py:   def greet(self): return "admin"
来源：http://uku.tian-w.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ohc.hnqzz.top

JS:   greet() { return "admin"; }
来源：http://pcp.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://ejd.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://put.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tmq.cdnleiting.top

Ruby: def greet; "admin"; end
来源：http://oge.yangfankeji.com

C#:   public override string Greet() => "admin";
来源：http://vkx.yueranfly.top

[G07] 调用父类方法
来源：http://kha.shuidangran.top

Py:   super().greet()
来源：http://yom.dashuyun.cn

PHP:  parent::greet();
来源：http://exm.snrcjt.cn

JS:   super.greet();
来源：http://upt.mhx1999.top

TS:   super.greet();
来源：http://qtq.guowangkeji.top

Java: super.greet();
来源：http://lwe.shanyushiyangtech.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://miw.cashguo.top

Ruby: super
来源：http://vhd.gotoacloud.top

C#:   base.Greet();
来源：http://ocw.vqdsnc.cn

[G08] 静态方法与属性
来源：http://hnc.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iht.fzhhl.top

PHP:  public static function f() {}
来源：http://evl.daxiang520.top

JS:   static f() {}
来源：http://mvx.zhongyouzk.top

TS:   static f(): void {}
来源：http://ryd.jinyuanbaomall.cn

Java: static void f() {}
来源：http://gwc.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://von.hysaishi.cn

Ruby: def self.f; end
来源：http://arm.havefunace.top

C#:   public static void F() {}
来源：http://lrf.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://umo.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://qos.sjlbkw.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xro.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vyh.hnxiangtu.top

TS:   interface Shape { area(): number; }
来源：http://fnd.gogol.net.cn

Java: interface Shape { double area(); }
来源：http://ayf.zdbjq.cn

Go:   type Shape interface { Area() float64 }
来源：http://sfz.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tte.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://oqn.zycfv.cn

[G10] 访问控制
来源：http://svv.yj202588.top

Py:   约定 _protected / __private（不强制）
来源：http://yaq.zhiwuduotai.top

PHP:  public / protected / private
来源：http://xii.gzhubu.top

JS:   #private 字段；其余公开
来源：http://mka.xinyue.icu

TS:   public / protected / private
来源：http://haa.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://lou.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pan.cheryme.top

Ruby: public / protected / private
来源：http://kii.sweek.top

C#:   public / protected / private / internal
来源：http://hew.dianchejie.cn

[G11] getter / setter
来源：http://okw.fzhhl.top

Py:   @property 与 @x.setter
来源：http://yiz.zhaomingkeji.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://wra.sxryk.cn

JS:   get name() { return this._name; }
来源：http://mgn.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://tft.zhoulong.xyz

Java: public String getName() { return name; }
来源：http://gba.jqgfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qze.shzxlz.cn

Ruby: attr_accessor :name
来源：http://mpz.zhoulong.xyz

C#:   public string Name { get; set; }
来源：http://yqg.hnqzz.top

[G12] 对象转字符串
来源：http://lrl.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://ebf.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cok.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://acw.hesvh.cn

TS:   toString(): string { return this.name; }
来源：http://djf.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://ywj.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://xvg.hcnkem.com

Ruby: def to_s; @name; end
来源：http://isv.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://sne.ybcxt.top

[G13] 判断对象类型
来源：http://mbs.yj202588.top

Py:   isinstance(u, User)
来源：http://lfy.tian-w.cn

PHP:  $u instanceof User
来源：http://rta.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://sfw.sweek.top

TS:   u instanceof User
来源：http://buu.gogol.net.cn

Java: u instanceof User
来源：http://xqa.jqgfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tay.ydzc1.top

Ruby: u.is_a?(User)
来源：http://iha.svipenyu.cn

C#:   u is User
来源：http://ndg.zhaomingkeji.xyz

[G14] 数据类 / record
来源：http://qfy.zhongyouzk.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sjj.xziqi.cn

PHP:  // 用 readonly 属性模拟
来源：http://tze.andypj.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://bek.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://ehh.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://wvq.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://jun.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://huu.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://haz.xinyue.icu

[G15] 枚举
来源：http://itk.fehbvm.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://skj.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hxc.epnwcf.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ymz.zhixingplan.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pns.gotoacloud.top

Java: enum Color { RED, GREEN }
来源：http://aij.shanyushiyangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hul.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://mzo.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wkg.fengsongda.top

[G16] 对象转数组 / 字典
来源：http://fkx.daria6918.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vwy.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://ica.tianlin.xyz

JS:   Object.entries(obj)
来源：http://cza.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://krl.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gps.jinqigfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dzw.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://bto.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://dnd.fehbvm.com

================================================================================
来源：http://agp.gzhubu.top

H. 异常与错误处理
来源：http://zti.shanyushiyangtech.top

================================================================================
来源：http://scr.ppjwa.cn

[H01] try / catch 基础
来源：http://wjs.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kji.xuanzx.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://czt.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ywu.yfazqb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yeb.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wbf.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qjm.jqgufenzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://owc.zdqjudy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ayf.jinqigfzy.top

[H02] finally / ensure 收尾
来源：http://mdc.zdbjq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sen.jqgufenzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nli.daxiang520.top

JS:   try { f(); } finally { cleanup(); }
来源：http://off.jyoumei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kjh.ybcxt.top

Java: try { f(); } finally { cleanup(); }
来源：http://dlw.fanxiaobao.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://mwr.dianchejie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rsf.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ibw.jianghu66.top

[H03] 主动抛出异常
来源：http://xwt.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://qkn.hywenlv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ybn.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://rwa.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://mhy.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uti.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wfq.yangfankeji.com

Ruby: raise ArgumentError, "错误信息"
来源：http://fas.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://enh.sxryk.cn

[H04] 自定义异常类型
来源：http://flv.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://xwq.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tbf.yongpay.top

JS:   class MyError extends Error {}
来源：http://cfa.xziqi.cn

TS:   class MyError extends Error {}
来源：http://vxh.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://rja.cheryme.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jpg.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://cpu.zdqjudy.top

C#:   class MyException : Exception {}
来源：http://fmo.sufxvd.cn

[H05] 捕获特定类型
来源：http://qjk.chenjidiqi.icu

Py:   except ValueError as e:
来源：http://snc.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://okx.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://kqy.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://uwe.nanxuanxn.top

Java: catch (IOException | SQLException e) {}
来源：http://npr.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uel.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://zph.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qrr.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://ipj.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://upw.gotoacloud.top

PHP:  $v = $d["k"] ?? null;
来源：http://kzg.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://acx.fktsv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ggj.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://byy.dashuyun.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lhn.zycfv.cn

Ruby: d&.dig(:a, :b)
来源：http://mqa.daxiang520.top

C#:   obj?.A?.B ?? default
来源：http://udt.ehwqpu.com

[H07] 断言
来源：http://mpg.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://ajg.ybcxt.top

PHP:  assert($x > 0);
来源：http://nba.uphjek.com

JS:   console.assert(x > 0);
来源：http://qey.xingfuxueyuan.xyz

TS:   console.assert(x > 0);
来源：http://mdk.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://izh.xinyue.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://naa.0kj1m.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uuw.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://wnv.bbcook.cn

[H08] 获取错误信息与堆栈
来源：http://vme.zhoulong.xyz

Py:   str(e);  traceback.format_exc()
来源：http://jri.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kih.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://eid.sxryk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zcj.andypj.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://qeo.vehdjk.com

Go:   err.Error()
来源：http://joe.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://mca.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://oyl.redwolf501.top

[H09] 带错误码的异常
来源：http://zlk.quarkkingdee.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uxy.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ret.yueranfly.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aox.jinyuanbaomall.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dfh.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hkl.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gtq.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xoh.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ihc.yongpay.top

[H10] 资源自动释放
来源：http://rfu.bbcook.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xmt.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://srg.cashguo.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ncl.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://chx.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eky.meibo888.top

Go:   defer f.Close()
来源：http://jjd.ctjpmb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jlt.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zus.fehbvm.com

================================================================================
来源：http://tiw.jyoumei.cn

I. 正则表达式
来源：http://qnp.jyoumei.cn

================================================================================
来源：http://iah.ybcxt.top

[I01] 判断是否匹配
来源：http://cyf.chenlongwang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://smg.bjfxy.top

PHP:  preg_match('/\d+/', $s);
来源：http://kul.cheryme.top

JS:   /\d+/.test(s)
来源：http://cvl.tanke756.top

TS:   /\d+/.test(s)
来源：http://tke.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cwm.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jsg.dianchejie.cn

Ruby: s.match?(/\d+/)
来源：http://ehj.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mvu.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://jvc.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://drw.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rok.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mhz.zhongyouzk.top

TS:   s.match(/\d+/g)
来源：http://lky.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://irg.xziqi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vtz.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://dte.zdqjudy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sin.yueranfly.top

[I03] 提取捕获分组
来源：http://blg.zdqjudy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kti.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hsd.chenjidiqi.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yrw.ybcxt.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hfj.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ouj.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kan.yj20258888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bvd.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vwg.zhongyouzk.top

[I04] 正则替换
来源：http://vxd.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wjg.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://exq.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://yds.0kj1m.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hmj.cucudq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dcw.hammf.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wsq.zhaomingkeji.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://xim.zhoulong.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uyu.yueranfly.top

[I05] 按正则拆分
来源：http://ucn.jinyuanbaomall.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gum.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tvc.kuanghao11.cn

JS:   s.split(/\s*,\s*/)
来源：http://gzv.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://oji.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://ait.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ija.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kdw.yanxiufei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://etm.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aug.fzhhl.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bhf.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oib.jianghu66.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://abj.sysykeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jfo.zdbjq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://asv.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mkt.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lzi.jyoumei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wfj.aizwys.cn

[I07] 忽略大小写与多行模式
来源：http://hsc.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bkg.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hco.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yeb.kuanghao11.cn

TS:   /error/gim
来源：http://prm.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mtw.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yqe.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://ome.jinyuanbaomall.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jfp.chenjidiqi.icu

[I08] 贪婪与非贪婪匹配
来源：http://wum.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sci.hfpthk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nbl.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uvm.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cgq.tianlin.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://vgh.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hgl.nwbrower.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nup.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://elv.jqgufenzy.top

================================================================================
来源：http://udc.aizwys.cn

J. 日期与时间
来源：http://rcx.jinqigfzy.top

================================================================================
来源：http://xqf.tarul.cn

[J01] 获取当前时间
来源：http://rpc.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gbt.ydzc1.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yxu.pycfn.com

JS:   new Date();  Date.now()
来源：http://xrn.fktsv.cn

TS:   new Date();  Date.now()
来源：http://tbu.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://tby.fanxiaobao.xyz

Go:   time.Now()
来源：http://xrf.hcnkem.com

Ruby: Time.now
来源：http://qcq.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mcy.jiagoushi.top

[J02] 格式化输出
来源：http://tfa.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aif.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vkg.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wrg.hysaishi.cn

TS:   d.toISOString()
来源：http://jan.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gzf.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zaf.jqgufenzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cqx.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xhi.iojbl.cn

[J03] 字符串解析为日期
来源：http://sko.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mfa.0kj1m.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xuk.fzhhl.top

JS:   new Date("2024-01-02")
来源：http://oxt.dashuyun.cn

TS:   new Date("2024-01-02")
来源：http://qll.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://qrc.zycfv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gbn.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://rvb.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ora.smart0.xyz

[J04] 时间戳与日期互转
来源：http://iuj.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ooa.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://otr.sxryk.cn


<!-- 参考信息 -->