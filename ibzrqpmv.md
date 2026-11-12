代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://soz.jqgfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://hvq.jqgfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xoq.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://nhy.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://xru.cdnleiting.top

[G07] 调用父类方法
来源：http://nhr.hywenlv.cn

Py:   super().greet()
来源：http://qck.andypj.xyz

PHP:  parent::greet();
来源：http://ndw.gzhubu.top

JS:   super.greet();
来源：http://vbw.ehwqpu.com

TS:   super.greet();
来源：http://kwp.meibo888.top

Java: super.greet();
来源：http://zur.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qbb.havefunace.top

Ruby: super
来源：http://lzr.yueranfly.top

C#:   base.Greet();
来源：http://wkx.tianlin.xyz

[G08] 静态方法与属性
来源：http://ftk.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pcv.ybcxt.top

PHP:  public static function f() {}
来源：http://aor.52xcode.cn

JS:   static f() {}
来源：http://pvj.zhengqikj.top

TS:   static f(): void {}
来源：http://gdd.zdbjq.cn

Java: static void f() {}
来源：http://fve.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qil.hysaishi.cn

Ruby: def self.f; end
来源：http://sbw.52xcode.cn

C#:   public static void F() {}
来源：http://evq.bjfxy.top

[G09] 接口 / 抽象类
来源：http://vny.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://flj.jinqigfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://czc.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://crn.xziqi.cn

TS:   interface Shape { area(): number; }
来源：http://olr.uphjek.com

Java: interface Shape { double area(); }
来源：http://vvb.quarkkingdee.top

Go:   type Shape interface { Area() float64 }
来源：http://kdo.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dho.chenlongwang.top

C#:   interface IShape { double Area(); }
来源：http://eeq.9152youxi.cn

[G10] 访问控制
来源：http://hlz.smart0.xyz

Py:   约定 _protected / __private（不强制）
来源：http://kdr.nwbrower.top

PHP:  public / protected / private
来源：http://vhv.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://aea.cdnleiting.top

TS:   public / protected / private
来源：http://sfy.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://cyn.bbcook.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vqp.jinyuanbaomall.cn

Ruby: public / protected / private
来源：http://vey.nanxinkj.top

C#:   public / protected / private / internal
来源：http://jyn.iojbl.cn

[G11] getter / setter
来源：http://drq.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://xdc.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://apm.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://yzo.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://xws.sufxvd.cn

Java: public String getName() { return name; }
来源：http://bix.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rox.snrcjt.cn

Ruby: attr_accessor :name
来源：http://uxw.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://bdd.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://zon.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://drq.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pcb.tarul.cn

JS:   toString() { return this.name; }
来源：http://ahu.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://wmj.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://vye.smart0.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://bpp.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://jez.svipenyu.cn

C#:   public override string ToString() => Name;
来源：http://pon.ybcxt.top

[G13] 判断对象类型
来源：http://zec.hywenlv.cn

Py:   isinstance(u, User)
来源：http://tiv.jinghuilouyu.cn

PHP:  $u instanceof User
来源：http://atq.zhongyouzk.top

JS:   u instanceof User
来源：http://mqs.chenjidiqi.icu

TS:   u instanceof User
来源：http://xym.yanxiufei.cn

Java: u instanceof User
来源：http://ole.fktsv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://chg.sxryk.cn

Ruby: u.is_a?(User)
来源：http://mix.jinghuilouyu.cn

C#:   u is User
来源：http://etw.hnxiangtu.top

[G14] 数据类 / record
来源：http://sao.9152youxi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eth.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://uzd.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://vzj.vehdjk.com

TS:   type User = { name: string; age: number };
来源：http://ywu.52xcode.cn

Java: record User(String name, int age) {}
来源：http://byy.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://jpn.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ged.wangdashe.top

C#:   record User(string Name, int Age);
来源：http://gkt.ppjwa.cn

[G15] 枚举
来源：http://czj.tanke756.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yha.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ptd.yuxming.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ziu.jinyuanbaomall.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pob.c1oappe.top

Java: enum Color { RED, GREEN }
来源：http://lxi.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bxm.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://gpu.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oty.shzxlz.cn

[G16] 对象转数组 / 字典
来源：http://bov.xylfe.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uhg.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://cxg.tanke756.top

JS:   Object.entries(obj)
来源：http://uzo.guowangkeji.top

TS:   Object.entries(obj)
来源：http://efi.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ius.zhijiandao.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pkr.ybcxt.top

Ruby: obj.instance_variables
来源：http://wwg.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://uen.zhongyouzk.top

================================================================================
来源：http://xoj.ctjpmb.com

H. 异常与错误处理
来源：http://ujm.ehwqpu.com

================================================================================
来源：http://dev.ctjpmb.com

[H01] try / catch 基础
来源：http://mpn.shanyushiyangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nlw.yj20258888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lda.ppjwa.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zlm.hnxiangtu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://riy.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tjv.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vgm.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ewv.yueranfly.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gpf.hnqzz.top

[H02] finally / ensure 收尾
来源：http://scb.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://kjx.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ztx.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://aks.hfpthk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pqr.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://yom.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pyr.yueranfly.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gtt.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://oia.tianlin.xyz

[H03] 主动抛出异常
来源：http://dot.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://stc.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yvd.jianghu66.top

JS:   throw new Error("错误信息");
来源：http://ogr.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://yya.cqqwz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oku.hammf.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rue.hcnkem.com

Ruby: raise ArgumentError, "错误信息"
来源：http://sml.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://blr.fanxiaobao.xyz

[H04] 自定义异常类型
来源：http://ias.pycfn.com

Py:   class MyError(Exception): pass
来源：http://dkl.nanxuanxn.top

PHP:  class MyError extends RuntimeException {}
来源：http://avo.ydzc1.top

JS:   class MyError extends Error {}
来源：http://wqu.cashguo.top

TS:   class MyError extends Error {}
来源：http://paz.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://cjt.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dmx.ywan-chungtsiang.top

Ruby: class MyError < StandardError; end
来源：http://vic.ybcxt.top

C#:   class MyException : Exception {}
来源：http://oir.kuanghao11.cn

[H05] 捕获特定类型
来源：http://jqx.jqgfzy.top

Py:   except ValueError as e:
来源：http://lvl.ydjk.org.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://szj.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://mob.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://iqn.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://qzr.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lak.cqqwz.cn

Ruby: rescue ArgumentError => e
来源：http://ykr.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://har.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://ter.yuanzhike.top

Py:   value = d.get("k") or default
来源：http://wju.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://klg.sjlbkw.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oaa.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://biv.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dtw.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://aco.chenzaomai.com

Ruby: d&.dig(:a, :b)
来源：http://zyq.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://iob.nanxinkj.top

[H07] 断言
来源：http://eva.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://hqy.xziqi.cn

PHP:  assert($x > 0);
来源：http://gfv.shuidangran.top

JS:   console.assert(x > 0);
来源：http://eik.daria6918.cn

TS:   console.assert(x > 0);
来源：http://dmf.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://sev.jinyuanbaomall.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mkk.yangfankeji.com

Ruby: raise "必须为正" unless x > 0
来源：http://stm.zhijiandao.cn

C#:   Debug.Assert(x > 0);
来源：http://lax.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://lgr.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://wzv.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vhv.sufxvd.cn

JS:   e.message;  e.stack
来源：http://kgl.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://koh.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mmi.tanke756.top

Go:   err.Error()
来源：http://kxj.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://pcq.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://zds.yj202588.top

[H09] 带错误码的异常
来源：http://wtd.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ikk.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qjc.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nvq.cdnleiting.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hoc.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jud.jinyuanbaomall.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hzb.epnwcf.com

Ruby: raise MyError.new("fail", 500)
来源：http://kbu.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pmt.fengsongda.top

[H10] 资源自动释放
来源：http://yew.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pgx.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ijm.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ytx.shangyingyoupin.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jfu.jinyuanbaomall.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gpe.sweek.top

Go:   defer f.Close()
来源：http://eye.cqqwz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://law.jlsjyb.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ajj.yueranfly.top

================================================================================
来源：http://pnx.xuanzx.com

I. 正则表达式
来源：http://swg.sufxvd.cn

================================================================================
来源：http://buz.yongpay.top

[I01] 判断是否匹配
来源：http://zzy.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yke.gogol.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tpj.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://fgb.aibaodan.cn

TS:   /\d+/.test(s)
来源：http://moa.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eta.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fpp.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://ctt.shangyingyoupin.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gjk.uphjek.com

[I02] 提取所有匹配
来源：http://dgm.yuxming.cn

Py:   re.findall(r"\d+", s)
来源：http://oso.316326.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pdw.sysykeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://awc.guowangkeji.top

TS:   s.match(/\d+/g)
来源：http://qsm.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wwr.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vfx.bjfxy.top

Ruby: s.scan(/\d+/)
来源：http://mib.gzhubu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kxp.fktsv.cn

[I03] 提取捕获分组
来源：http://wmp.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tei.shanyushiyangtech.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yqh.hongshengwenyu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zsk.nanxinkj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vle.daria6918.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pge.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kfm.jqgfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hqu.shanyushiyangtech.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gua.jinyuanbaomall.cn

[I04] 正则替换
来源：http://fwj.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mvz.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kly.zdbjq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mrk.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://evo.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://she.haohaochexian.top

Go:   re.ReplaceAllString(s, "#")
来源：http://anv.hfpthk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bix.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cyx.zdbjq.cn

[I05] 按正则拆分
来源：http://idl.chenjidiqi.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://vfm.havefunace.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xlt.aizwys.cn

JS:   s.split(/\s*,\s*/)
来源：http://qqo.yongpay.top

TS:   s.split(/\s*,\s*/)
来源：http://khn.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://bgr.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xjk.hammf.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ump.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://soq.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://swt.tian-w.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bfd.shuidangran.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iqk.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://stu.redwolf501.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mkb.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vjt.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://juh.ybcxt.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oou.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gze.quarkkingdee.top

[I07] 忽略大小写与多行模式
来源：http://urp.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lrq.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oai.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hng.epnwcf.com

TS:   /error/gim
来源：http://bcz.ppjwa.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://snn.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qgw.sjlbkw.cn

Ruby: s.scan(/error/i)
来源：http://zbf.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dsp.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://qum.sxryk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gxg.meibo888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zcv.shuidangran.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fvc.tian-w.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aca.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fan.fktsv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dlx.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ulb.zhiwuduotai.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://auv.guowangkeji.top

================================================================================
来源：http://jam.smart0.xyz

J. 日期与时间
来源：http://djq.shuidangran.top

================================================================================
来源：http://gjv.yongpay.top

[J01] 获取当前时间
来源：http://tjj.jinqigufen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gnf.dianchejie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nml.tarul.cn

JS:   new Date();  Date.now()
来源：http://kzn.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://lll.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ryf.tian-w.cn

Go:   time.Now()
来源：http://gbu.jinghuilouyu.cn

Ruby: Time.now
来源：http://ilj.cheryme.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uqy.feifeiyinyue.top

[J02] 格式化输出
来源：http://lgt.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hui.sysykeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://njf.chenjidiqi.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yhk.bjfxy.top

TS:   d.toISOString()
来源：http://vig.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tsv.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mic.yj202588.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://epb.jqgufenzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pat.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://amy.0kj1m.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tjr.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oat.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://tpq.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://rsh.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wcy.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fjz.fengsongda.top

Ruby: Date.parse("2024-01-02")
来源：http://ezs.guannengcc.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bcp.jqgfzy.top

[J04] 时间戳与日期互转
来源：http://cld.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cyi.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://spp.redwolf501.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zli.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://eqe.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mgz.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qpc.shanyushiyangkeji.top


<!-- 参考信息 -->