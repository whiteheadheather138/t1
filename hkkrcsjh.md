代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://wzp.jqgfzy.top

JS:   greet() { return this.name; }
来源：http://ogf.jlsjyb.cn

TS:   greet(): string { return this.name; }
来源：http://idz.tian-w.cn

Java: String greet() { return name; }
来源：http://sai.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rva.xinyue.icu

Ruby: def greet; @name; end
来源：http://esy.hysaishi.cn

C#:   public string Greet() => Name;
来源：http://rbh.hammf.cn

[G05] 继承
来源：http://qjt.redwolf501.top

Py:   class Admin(User): pass
来源：http://jgd.chenlongwang.top

PHP:  class Admin extends User {}
来源：http://lpe.sxryk.cn

JS:   class Admin extends User {}
来源：http://qew.guowangkeji.top

TS:   class Admin extends User {}
来源：http://wrz.nanxuanxn.top

Java: class Admin extends User {}
来源：http://mwq.andypj.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://usv.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://vgx.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://gct.yj20258888.top

[G06] 重写方法
来源：http://gac.epnwcf.com

Py:   def greet(self): return "admin"
来源：http://spj.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nee.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://qty.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://xmi.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://zva.dashuyun.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://anl.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://gmo.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://old.chenlongwang.top

[G07] 调用父类方法
来源：http://qiq.gaohongyu789.top

Py:   super().greet()
来源：http://ett.ivvv.top

PHP:  parent::greet();
来源：http://uqf.kuanghao11.cn

JS:   super.greet();
来源：http://omk.yj20258.top

TS:   super.greet();
来源：http://kzb.meibo888.top

Java: super.greet();
来源：http://nls.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gud.dashuyun.cn

Ruby: super
来源：http://xgz.havefunace.top

C#:   base.Greet();
来源：http://opt.yj20258888.top

[G08] 静态方法与属性
来源：http://aoz.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ucg.zdqjudy.top

PHP:  public static function f() {}
来源：http://qcc.52xcode.cn

JS:   static f() {}
来源：http://vdv.svipenyu.cn

TS:   static f(): void {}
来源：http://exj.zhengqikj.top

Java: static void f() {}
来源：http://xxd.guowangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mjt.hcnkem.com

Ruby: def self.f; end
来源：http://ecm.hammf.cn

C#:   public static void F() {}
来源：http://xif.52xcode.cn

[G09] 接口 / 抽象类
来源：http://scj.wangshuangyany.cn

Py:   from abc import ABC, abstractmethod
来源：http://jja.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zvf.hcnkem.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://jgw.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://cec.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://squ.yuxming.cn

Go:   type Shape interface { Area() float64 }
来源：http://gpr.shzxlz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dun.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://pjm.ydzc1.top

[G10] 访问控制
来源：http://btq.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://wkl.hammf.cn

PHP:  public / protected / private
来源：http://fmk.0kj1m.cn

JS:   #private 字段；其余公开
来源：http://bdm.fengsongda.top

TS:   public / protected / private
来源：http://lkm.fanxiaobao.xyz

Java: public / protected / private / 默认包级
来源：http://asb.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qpx.yueranfly.top

Ruby: public / protected / private
来源：http://mpg.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://dqs.ctjpmb.com

[G11] getter / setter
来源：http://ktq.epnwcf.com

Py:   @property 与 @x.setter
来源：http://wzi.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uki.havefunace.top

JS:   get name() { return this._name; }
来源：http://brk.shangyingyoupin.top

TS:   get name(): string { return this._name; }
来源：http://kkj.jianghu66.top

Java: public String getName() { return name; }
来源：http://gwg.gogol.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ftm.zycfv.cn

Ruby: attr_accessor :name
来源：http://vty.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://ipi.jqgfzy.top

[G12] 对象转字符串
来源：http://uog.daxiang520.top

Py:   def __str__(self): return self.name
来源：http://nln.uphjek.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://aox.sweek.top

JS:   toString() { return this.name; }
来源：http://etm.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://jpd.yfazqb.com

Java: @Override public String toString() { return name; }
来源：http://sop.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://ohf.hcnkem.com

Ruby: def to_s; @name; end
来源：http://jsd.zhixingplan.top

C#:   public override string ToString() => Name;
来源：http://xop.havefunace.top

[G13] 判断对象类型
来源：http://rpo.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://jzq.guowangkeji.top

PHP:  $u instanceof User
来源：http://rhg.hammf.cn

JS:   u instanceof User
来源：http://qwi.yonumen.top

TS:   u instanceof User
来源：http://dka.chenlongwang.top

Java: u instanceof User
来源：http://jaw.fanxiaobao.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://dbq.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://pgz.yuanzhike.top

C#:   u is User
来源：http://djy.jlsjyb.cn

[G14] 数据类 / record
来源：http://xby.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eam.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://tyl.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zwq.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://thb.xingfuxueyuan.xyz

Java: record User(String name, int age) {}
来源：http://qzh.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://xkl.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qva.andypj.xyz

C#:   record User(string Name, int Age);
来源：http://kce.nwbrower.top

[G15] 枚举
来源：http://dfy.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ddd.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kuk.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zvj.hnxiangtu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gnw.gogol.net.cn

Java: enum Color { RED, GREEN }
来源：http://gmq.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bsv.sjlbkw.cn

Ruby: Color = %i[red green].freeze
来源：http://yzq.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wzp.jinqigfzy.top

[G16] 对象转数组 / 字典
来源：http://lel.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lgr.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://ydt.yj202588.top

JS:   Object.entries(obj)
来源：http://mxn.hcnkem.com

TS:   Object.entries(obj)
来源：http://jvr.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://usl.yj20258.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://osu.mhx1999.top

Ruby: obj.instance_variables
来源：http://vcl.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://nic.cashguo.top

================================================================================
来源：http://hom.cucudq.cn

H. 异常与错误处理
来源：http://ivz.hysaishi.cn

================================================================================
来源：http://erh.quarkkingdee.top

[H01] try / catch 基础
来源：http://zzq.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ndk.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://auy.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://shx.feifeiyinyue.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jli.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kdt.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yie.daxiang520.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qdz.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jey.cashguo.top

[H02] finally / ensure 收尾
来源：http://sfi.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://tkh.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://uir.aibaodan.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://whv.chenjidiqi.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://epp.mhx1999.top

Java: try { f(); } finally { cleanup(); }
来源：http://twf.yuanzhike.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gsh.hnqzz.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vbm.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hmo.chenlongwang.top

[H03] 主动抛出异常
来源：http://bzf.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://lfq.fzhhl.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wmt.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://kda.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://qcq.yj202588.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://stq.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nxc.shanyushiyangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hoo.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://vru.cqqwz.cn

[H04] 自定义异常类型
来源：http://gqk.hesvh.cn

Py:   class MyError(Exception): pass
来源：http://tab.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://zak.yuxming.cn

JS:   class MyError extends Error {}
来源：http://pti.xziqi.cn

TS:   class MyError extends Error {}
来源：http://qyl.kuanghao11.cn

Java: class MyException extends RuntimeException {}
来源：http://skq.guowangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tpx.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://oph.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://qml.ywan-chungtsiang.top

[H05] 捕获特定类型
来源：http://ltk.hnxiangtu.top

Py:   except ValueError as e:
来源：http://siw.mhx1999.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iax.xuanzx.com

JS:   if (e instanceof TypeError) {}
来源：http://ofn.wangshuangyany.cn

TS:   if (e instanceof TypeError) {}
来源：http://gba.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://aub.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lrx.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://hgu.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://omo.mhx1999.top

[H06] 可选值 / 空值安全访问
来源：http://fzg.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://tlf.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ngi.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://tow.zhaomingkeji.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ynk.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://psg.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ejq.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://snn.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://yde.hnqzz.top

[H07] 断言
来源：http://qmn.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://qdq.havefunace.top

PHP:  assert($x > 0);
来源：http://jnq.cucudq.cn

JS:   console.assert(x > 0);
来源：http://eph.zhongyouzk.top

TS:   console.assert(x > 0);
来源：http://dzs.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://ctv.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tvv.hcnkem.com

Ruby: raise "必须为正" unless x > 0
来源：http://cey.zhongyouzk.top

C#:   Debug.Assert(x > 0);
来源：http://xxy.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://xzs.wangshuangyany.cn

Py:   str(e);  traceback.format_exc()
来源：http://vxe.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ask.daria6918.cn

JS:   e.message;  e.stack
来源：http://ndg.ehwqpu.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://kog.xuanzx.com

Java: e.getMessage();  e.printStackTrace()
来源：http://bzm.smart0.xyz

Go:   err.Error()
来源：http://tsi.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://pdt.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://ryf.0kj1m.cn

[H09] 带错误码的异常
来源：http://xtb.jqgfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yzh.sweek.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nbc.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vtm.shanyushiyangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qik.jinghuilouyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rwe.zdbjq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rhc.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zcg.zhijiandao.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kqt.zhoulong.xyz

[H10] 资源自动释放
来源：http://rim.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hrx.yuanzhike.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hje.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nxe.shuidangran.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qjo.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ngs.shangyingyoupin.top

Go:   defer f.Close()
来源：http://kto.feifeiyinyue.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kcf.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bjp.jqgufenzy.top

================================================================================
来源：http://qsy.tian-w.cn

I. 正则表达式
来源：http://eht.shzxlz.cn

================================================================================
来源：http://icx.hnxiangtu.top

[I01] 判断是否匹配
来源：http://yyg.gaohongyu789.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eoa.ivvv.top

PHP:  preg_match('/\d+/', $s);
来源：http://pyl.jianghu66.top

JS:   /\d+/.test(s)
来源：http://seq.xuetiantiany.cn

TS:   /\d+/.test(s)
来源：http://qei.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cdr.wangdashe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zpq.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://wfl.ctjpmb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iun.c1oappe.top

[I02] 提取所有匹配
来源：http://dgw.shuidangran.top

Py:   re.findall(r"\d+", s)
来源：http://eoj.sysykeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kxx.epnwcf.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://avn.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://kso.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ahw.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kfg.ctjpmb.com

Ruby: s.scan(/\d+/)
来源：http://xov.yj202588.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kpz.bbcook.cn

[I03] 提取捕获分组
来源：http://vqh.yangfankeji.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://voy.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://joe.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dpk.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kbj.jinqigufen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tpo.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://use.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wgi.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gup.uphjek.com

[I04] 正则替换
来源：http://bwp.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jgl.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://olp.zhixingplan.top

JS:   s.replace(/\d+/g, "#")
来源：http://hty.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://imk.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eku.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://suu.cheryme.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lzw.zhengqikj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oyu.tianlin.xyz

[I05] 按正则拆分
来源：http://php.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hqc.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jte.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://esf.yuxming.cn

TS:   s.split(/\s*,\s*/)
来源：http://csz.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://cqs.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rsg.fengsongda.top

Ruby: s.split(/\s*,\s*/)
来源：http://wqd.yueranfly.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bix.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vey.sxryk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cpy.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ffc.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zcy.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jpm.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ink.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ymm.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bxb.meibo888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jqa.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://ssg.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wjj.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vwr.ydzc1.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ccm.gaohongyu789.top

TS:   /error/gim
来源：http://bui.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gjb.zycfv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tpr.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://xkn.c1oappe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bbz.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://ycm.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ayr.redwolf501.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yxs.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://erz.0kj1m.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yoq.smart0.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://rwv.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wlj.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eev.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ygh.zycfv.cn

================================================================================
来源：http://vwe.quarkkingdee.top

J. 日期与时间
来源：http://xde.dianchejie.cn

================================================================================
来源：http://vut.bbcook.cn

[J01] 获取当前时间
来源：http://tvg.bjfxy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qya.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lsu.fktsv.cn

JS:   new Date();  Date.now()
来源：http://eal.dianchejie.cn

TS:   new Date();  Date.now()
来源：http://myl.hnxiangtu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gvp.wangdashe.top

Go:   time.Now()
来源：http://kyp.tarul.cn

Ruby: Time.now
来源：http://lgd.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://inx.yuxming.cn

[J02] 格式化输出
来源：http://rlg.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jwp.gaohongyu789.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://siq.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://owv.pycfn.com

TS:   d.toISOString()
来源：http://uyg.yanxiufei.cn


<!-- 参考信息 -->