代发 wailian999

Java: class Admin extends User {}
来源：http://rtq.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uet.pycfn.com

Ruby: class Admin < User; end
来源：http://jhs.xingfuxueyuan.xyz

C#:   class Admin : User {}
来源：http://bcr.daxiang520.top

[G06] 重写方法
来源：http://kou.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://qgt.zhengqikj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qqz.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://dmr.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://hee.svipenyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://zfu.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uoi.hfpthk.cn

Ruby: def greet; "admin"; end
来源：http://svd.gotoacloud.top

C#:   public override string Greet() => "admin";
来源：http://iog.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://ywa.jianghu66.top

Py:   super().greet()
来源：http://rcb.hfpthk.cn

PHP:  parent::greet();
来源：http://hqv.daxiang520.top

JS:   super.greet();
来源：http://mmq.tianlin.xyz

TS:   super.greet();
来源：http://jig.yongpay.top

Java: super.greet();
来源：http://fcq.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://drf.shuidangran.top

Ruby: super
来源：http://uir.yangfankeji.com

C#:   base.Greet();
来源：http://smw.smart0.xyz

[G08] 静态方法与属性
来源：http://aqp.jinqigufen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rgt.quarkkingdee.top

PHP:  public static function f() {}
来源：http://olv.sysykeji.top

JS:   static f() {}
来源：http://snb.fktsv.cn

TS:   static f(): void {}
来源：http://lwv.yongpay.top

Java: static void f() {}
来源：http://xcd.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://zei.316326.xyz

Ruby: def self.f; end
来源：http://svb.gaohongyu789.top

C#:   public static void F() {}
来源：http://rxr.pengpengdd.cyou

[G09] 接口 / 抽象类
来源：http://iui.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://azw.ehwqpu.com

PHP:  interface Shape { public function area(): float; }
来源：http://yum.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tej.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://mdp.ehwqpu.com

Java: interface Shape { double area(); }
来源：http://nvh.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://gfp.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://igf.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://ckn.gaohongyu789.top

[G10] 访问控制
来源：http://xkp.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://hid.pycfn.com

PHP:  public / protected / private
来源：http://jzn.0kj1m.cn

JS:   #private 字段；其余公开
来源：http://srk.hysaishi.cn

TS:   public / protected / private
来源：http://lcl.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://lhw.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yvm.shuidangran.top

Ruby: public / protected / private
来源：http://rwo.uphjek.com

C#:   public / protected / private / internal
来源：http://elu.yj20258888.top

[G11] getter / setter
来源：http://nfd.xinyue.icu

Py:   @property 与 @x.setter
来源：http://lma.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://pwl.havefunace.top

JS:   get name() { return this._name; }
来源：http://hsk.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://ffm.yj20258888.top

Java: public String getName() { return name; }
来源：http://dit.cqqwz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jcz.ybcxt.top

Ruby: attr_accessor :name
来源：http://gnj.smart0.xyz

C#:   public string Name { get; set; }
来源：http://ltt.jlsjyb.cn

[G12] 对象转字符串
来源：http://evm.bbcook.cn

Py:   def __str__(self): return self.name
来源：http://dgt.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dci.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://spq.zhongyouzk.top

TS:   toString(): string { return this.name; }
来源：http://ily.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://zbm.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://gle.jqgufenzy.top

Ruby: def to_s; @name; end
来源：http://jax.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://tlh.xuanzx.com

[G13] 判断对象类型
来源：http://nrq.uphjek.com

Py:   isinstance(u, User)
来源：http://zdu.andypj.xyz

PHP:  $u instanceof User
来源：http://eik.9152youxi.cn

JS:   u instanceof User
来源：http://pzv.316326.xyz

TS:   u instanceof User
来源：http://xab.hcnkem.com

Java: u instanceof User
来源：http://cuf.pycfn.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://jvd.ydzc1.top

Ruby: u.is_a?(User)
来源：http://als.shuidangran.top

C#:   u is User
来源：http://trl.guowangkeji.top

[G14] 数据类 / record
来源：http://cca.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ckd.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://eft.shanyushiyangtech.top

JS:   // 无内置：普通类或对象字面量
来源：http://gkn.52xcode.cn

TS:   type User = { name: string; age: number };
来源：http://tiu.fzhhl.top

Java: record User(String name, int age) {}
来源：http://rmw.ppjwa.cn

Go:   type User struct { Name string; Age int }
来源：http://wxa.gaohongyu789.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xvd.daria6918.cn

C#:   record User(string Name, int Age);
来源：http://egr.zdbjq.cn

[G15] 枚举
来源：http://ycf.hysaishi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hsk.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://uwm.0kj1m.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://weh.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fxm.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://ifq.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aym.uphjek.com

Ruby: Color = %i[red green].freeze
来源：http://vpe.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jwg.hcnkem.com

[G16] 对象转数组 / 字典
来源：http://ruc.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mkr.uphjek.com

PHP:  get_object_vars($obj);
来源：http://vqg.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://ymq.tarul.cn

TS:   Object.entries(obj)
来源：http://jrn.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xed.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ols.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://dgu.chenlongwang.top

C#:   // 用反射或 System.Text.Json
来源：http://hjd.wangdashe.top

================================================================================
来源：http://yfg.hnxiangtu.top

H. 异常与错误处理
来源：http://yxy.jlsjyb.cn

================================================================================
来源：http://esu.jyoumei.cn

[H01] try / catch 基础
来源：http://uxy.jianghu66.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mlj.yj20258888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ptw.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pht.cheryme.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bgy.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gpv.jqgfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fdk.cdnleiting.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ncu.fzhhl.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bnu.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://wod.yfazqb.com

Py:   try: f()⏎finally: cleanup()
来源：http://dpm.shanyushiyangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fpt.yanxiufei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ufu.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xoz.zdqjudy.top

Java: try { f(); } finally { cleanup(); }
来源：http://ccm.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kdi.yangfankeji.com

Ruby: begin; f; ensure; cleanup; end
来源：http://cwe.zhiwuduotai.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://srw.shzxlz.cn

[H03] 主动抛出异常
来源：http://gzs.vqdsnc.cn

Py:   raise ValueError("错误信息")
来源：http://yot.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://phb.zdbjq.cn

JS:   throw new Error("错误信息");
来源：http://mke.yj202588.top

TS:   throw new Error("错误信息");
来源：http://ezp.yonumen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://egg.chenzaomai.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://epi.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gzl.zhijiandao.cn

C#:   throw new ArgumentException("错误信息");
来源：http://aov.cashguo.top

[H04] 自定义异常类型
来源：http://qof.cucudq.cn

Py:   class MyError(Exception): pass
来源：http://hlg.uphjek.com

PHP:  class MyError extends RuntimeException {}
来源：http://ome.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://huu.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://kkg.sjlbkw.cn

Java: class MyException extends RuntimeException {}
来源：http://bsv.316326.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cog.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://swc.chenjidiqi.icu

C#:   class MyException : Exception {}
来源：http://oko.wangdashe.top

[H05] 捕获特定类型
来源：http://kff.52xcode.cn

Py:   except ValueError as e:
来源：http://izi.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vce.nanxinkj.top

JS:   if (e instanceof TypeError) {}
来源：http://nxo.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://pox.shuidangran.top

Java: catch (IOException | SQLException e) {}
来源：http://wwf.0kj1m.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oqh.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://tta.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://phj.jqgufenzy.top

[H06] 可选值 / 空值安全访问
来源：http://liu.shangyingyoupin.top

Py:   value = d.get("k") or default
来源：http://qva.nanxinkj.top

PHP:  $v = $d["k"] ?? null;
来源：http://kch.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://yix.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://gaa.guannengcc.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://odx.yuanzhike.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vut.jianghu66.top

Ruby: d&.dig(:a, :b)
来源：http://hlb.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://lef.gaohongyu789.top

[H07] 断言
来源：http://upz.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://rzo.ppjwa.cn

PHP:  assert($x > 0);
来源：http://zgc.nanxuanxn.top

JS:   console.assert(x > 0);
来源：http://fkl.cashguo.top

TS:   console.assert(x > 0);
来源：http://tkg.aizwys.cn

Java: assert x > 0 : "必须为正";
来源：http://qls.sweek.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wgk.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://nfx.zhongyouzk.top

C#:   Debug.Assert(x > 0);
来源：http://qsj.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://ldu.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://bep.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pht.uphjek.com

JS:   e.message;  e.stack
来源：http://nds.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://esi.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://spq.fehbvm.com

Go:   err.Error()
来源：http://wlx.tian-w.cn

Ruby: e.message;  e.backtrace
来源：http://aju.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://utn.meibo888.top

[H09] 带错误码的异常
来源：http://rkr.nwbrower.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xxn.bbcook.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lny.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://axn.shanyushiyangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lug.xziqi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aaw.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ifk.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://nol.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://cyv.smart0.xyz

[H10] 资源自动释放
来源：http://jng.yvedp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ygx.wangdashe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tis.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hqi.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://saw.cucudq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://unt.tarul.cn

Go:   defer f.Close()
来源：http://mkr.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qko.yuxming.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pie.sweek.top

================================================================================
来源：http://mtv.zhengqikj.top

I. 正则表达式
来源：http://tfj.meibo888.top

================================================================================
来源：http://jfn.zdbjq.cn

[I01] 判断是否匹配
来源：http://ibf.hfpthk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ult.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://krm.yonumen.top

JS:   /\d+/.test(s)
来源：http://xrh.daxiang520.top

TS:   /\d+/.test(s)
来源：http://reg.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eyt.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bsu.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://gsg.gogol.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sst.shuidangran.top

[I02] 提取所有匹配
来源：http://hsf.feifeiyinyue.top

Py:   re.findall(r"\d+", s)
来源：http://ygj.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cdo.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mgb.fktsv.cn

TS:   s.match(/\d+/g)
来源：http://jaq.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bfl.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qjh.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://elz.vehdjk.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ega.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://vgf.shzxlz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mer.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rtb.guannengcc.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vgm.svipenyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://idb.epnwcf.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ygh.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rnq.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vdu.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://psy.aibaodan.cn

[I04] 正则替换
来源：http://ors.yj20258.top

Py:   re.sub(r"\d+", "#", s)
来源：http://try.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://elx.ivvv.top

JS:   s.replace(/\d+/g, "#")
来源：http://glf.0kj1m.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uwf.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://xcn.zhaomingkeji.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://tsg.ppjwa.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qkl.tianlin.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vgx.jianghu66.top

[I05] 按正则拆分
来源：http://toq.daria6918.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uim.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fgn.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://aah.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://snf.zhiwuduotai.top

Java: s.split("\\s*,\\s*")
来源：http://ggn.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gzp.jianghu66.top

Ruby: s.split(/\s*,\s*/)
来源：http://opq.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ldx.tian-w.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gap.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yxm.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nxo.svipenyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qlk.ywan-chungtsiang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wdi.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wvh.yvedp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gee.pengpengdd.cyou

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rja.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nkx.zhiwuduotai.top

[I07] 忽略大小写与多行模式
来源：http://mlj.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gqp.dashuyun.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vwt.quarkkingdee.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qac.hesvh.cn

TS:   /error/gim
来源：http://fwu.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qmx.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xlr.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://obt.quarkkingdee.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oil.havefunace.top

[I08] 贪婪与非贪婪匹配
来源：http://qtt.ydjk.org.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bqf.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xjs.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zuy.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hzt.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://nbh.guowangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tdh.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qjk.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nyl.cheryme.top

================================================================================
来源：http://vly.zdqjudy.top

J. 日期与时间
来源：http://ycf.epnwcf.com

================================================================================
来源：http://lhb.zhongyouzk.top

[J01] 获取当前时间
来源：http://pqi.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://sqc.zdqjudy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://smz.xuetiantiany.cn

JS:   new Date();  Date.now()
来源：http://skq.hesvh.cn

TS:   new Date();  Date.now()
来源：http://vqi.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vyj.redwolf501.top

Go:   time.Now()
来源：http://lqb.jyoumei.cn

Ruby: Time.now
来源：http://opp.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hav.hywenlv.cn

[J02] 格式化输出
来源：http://tdm.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wwv.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kpe.ppjwa.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ofh.gogol.net.cn

TS:   d.toISOString()
来源：http://vle.redwolf501.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cnv.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kby.chenjidiqi.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kpv.c1oappe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zvb.tanke756.top

[J03] 字符串解析为日期
来源：http://aoc.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aum.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xsh.yj202588.top

JS:   new Date("2024-01-02")
来源：http://xsy.jianghu66.top

TS:   new Date("2024-01-02")
来源：http://ukg.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wlr.ehwqpu.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qig.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://aka.redwolf501.top


<!-- 参考信息 -->