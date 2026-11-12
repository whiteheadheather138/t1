代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://pma.yj20258888.top

[G03] 实例属性
来源：http://sjc.wangdashe.top

Py:   self.name = "x"
来源：http://zdo.tanke756.top

PHP:  public string $name = "x";
来源：http://arj.yuxming.cn

JS:   this.name = "x";
来源：http://gdo.yuanzhike.top

TS:   name: string = "x";
来源：http://uea.daxiang520.top

Java: private String name;
来源：http://lah.zycfv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mwg.redwolf501.top

Ruby: @name = "x"
来源：http://gkv.dashuyun.cn

C#:   public string Name { get; set; } = "x";
来源：http://ewt.nanxinkj.top

[G04] 定义方法
来源：http://xop.pycfn.com

Py:   def greet(self): return self.name
来源：http://nps.zhaomingkeji.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://lvw.c1oappe.top

JS:   greet() { return this.name; }
来源：http://fcl.hnqzz.top

TS:   greet(): string { return this.name; }
来源：http://xbp.havefunace.top

Java: String greet() { return name; }
来源：http://ski.xziqi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yoe.jinghuilouyu.cn

Ruby: def greet; @name; end
来源：http://vqq.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://lpw.andypj.xyz

[G05] 继承
来源：http://cuf.fktsv.cn

Py:   class Admin(User): pass
来源：http://xlz.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://nww.nwbrower.top

JS:   class Admin extends User {}
来源：http://ltu.yongpay.top

TS:   class Admin extends User {}
来源：http://rjs.sxryk.cn

Java: class Admin extends User {}
来源：http://cvz.yfazqb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sxv.fehbvm.com

Ruby: class Admin < User; end
来源：http://wsv.zhijiandao.cn

C#:   class Admin : User {}
来源：http://fax.redwolf501.top

[G06] 重写方法
来源：http://sko.fanxiaobao.xyz

Py:   def greet(self): return "admin"
来源：http://tyq.sysykeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cna.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://hwa.aizwys.cn

TS:   greet(): string { return "admin"; }
来源：http://zio.svipenyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://qnx.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nme.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://vno.zhongyouzk.top

C#:   public override string Greet() => "admin";
来源：http://ezj.aibaodan.cn

[G07] 调用父类方法
来源：http://sia.ywan-chungtsiang.top

Py:   super().greet()
来源：http://vnk.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://fsp.c1oappe.top

JS:   super.greet();
来源：http://yrp.pengpengdd.cyou

TS:   super.greet();
来源：http://cbf.smart0.xyz

Java: super.greet();
来源：http://omm.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ync.xuetiantiany.cn

Ruby: super
来源：http://ipc.redwolf501.top

C#:   base.Greet();
来源：http://umc.tian-w.cn

[G08] 静态方法与属性
来源：http://itx.snrcjt.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://taf.9152youxi.cn

PHP:  public static function f() {}
来源：http://tqf.pycfn.com

JS:   static f() {}
来源：http://lqz.hnxiangtu.top

TS:   static f(): void {}
来源：http://lln.epnwcf.com

Java: static void f() {}
来源：http://fwo.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://etb.xuanzx.com

Ruby: def self.f; end
来源：http://fjs.yangfankeji.com

C#:   public static void F() {}
来源：http://jeh.xuanzx.com

[G09] 接口 / 抽象类
来源：http://jpr.9152youxi.cn

Py:   from abc import ABC, abstractmethod
来源：http://ezs.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://qtq.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xdv.cheryme.top

TS:   interface Shape { area(): number; }
来源：http://ifb.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://doj.hesvh.cn

Go:   type Shape interface { Area() float64 }
来源：http://pim.cashguo.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ktg.iojbl.cn

C#:   interface IShape { double Area(); }
来源：http://aei.tian-w.cn

[G10] 访问控制
来源：http://ypw.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://bhk.9152youxi.cn

PHP:  public / protected / private
来源：http://ktf.nanxinkj.top

JS:   #private 字段；其余公开
来源：http://xqi.jinghuilouyu.cn

TS:   public / protected / private
来源：http://pyy.shanyushiyangkeji.top

Java: public / protected / private / 默认包级
来源：http://igr.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rcg.iojbl.cn

Ruby: public / protected / private
来源：http://vxv.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://chv.birdmap.top

[G11] getter / setter
来源：http://ujk.hcnkem.com

Py:   @property 与 @x.setter
来源：http://twm.ydzc1.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hku.jinyuanbaomall.cn

JS:   get name() { return this._name; }
来源：http://kip.52xcode.cn

TS:   get name(): string { return this._name; }
来源：http://wpg.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://omp.yueranfly.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fbn.chenlongwang.top

Ruby: attr_accessor :name
来源：http://gmu.316326.xyz

C#:   public string Name { get; set; }
来源：http://whq.snrcjt.cn

[G12] 对象转字符串
来源：http://qhm.zhengqikj.top

Py:   def __str__(self): return self.name
来源：http://xar.sysykeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://omp.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://rna.guowangkeji.top

TS:   toString(): string { return this.name; }
来源：http://spw.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://nip.zhaomingkeji.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://zee.zycfv.cn

Ruby: def to_s; @name; end
来源：http://yco.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://evb.yj20258888.top

[G13] 判断对象类型
来源：http://frc.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://vgs.aibaodan.cn

PHP:  $u instanceof User
来源：http://zpw.snrcjt.cn

JS:   u instanceof User
来源：http://oea.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://dfn.aizwys.cn

Java: u instanceof User
来源：http://hbh.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vxt.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://rky.yongpay.top

C#:   u is User
来源：http://pdo.316326.xyz

[G14] 数据类 / record
来源：http://lwr.pycfn.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mpt.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://irt.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://gmy.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://grf.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://vvs.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://ioe.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://okj.0kj1m.cn

C#:   record User(string Name, int Age);
来源：http://drs.daria6918.cn

[G15] 枚举
来源：http://aip.cdnleiting.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://guu.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kdw.kuanghao11.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dxj.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uci.hesvh.cn

Java: enum Color { RED, GREEN }
来源：http://ccq.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rdk.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://ylm.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yru.316326.xyz

[G16] 对象转数组 / 字典
来源：http://rzc.ppjwa.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rmp.jqgufenzy.top

PHP:  get_object_vars($obj);
来源：http://xqg.xingfuxueyuan.xyz

JS:   Object.entries(obj)
来源：http://oye.yangfankeji.com

TS:   Object.entries(obj)
来源：http://kzv.wangshuangyany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ubz.zhaomingkeji.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://yte.zdbjq.cn

Ruby: obj.instance_variables
来源：http://ney.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://sqk.xingfuxueyuan.xyz

================================================================================
来源：http://xno.sjlbkw.cn

H. 异常与错误处理
来源：http://hry.hfpthk.cn

================================================================================
来源：http://yzl.jqgufenzy.top

[H01] try / catch 基础
来源：http://haw.xuetiantiany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ovt.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rdr.hammf.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gbi.nanxuanxn.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tth.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ebn.ydjk.org.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gey.ywan-chungtsiang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gbg.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cgw.guannengcc.top

[H02] finally / ensure 收尾
来源：http://hra.chenlongwang.top

Py:   try: f()⏎finally: cleanup()
来源：http://pdb.hnqzz.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://prs.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://stf.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://vrw.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://ipk.ydzc1.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kjd.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jho.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://osk.cucudq.cn

[H03] 主动抛出异常
来源：http://wyf.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://ehz.nanxuanxn.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ymv.wangdashe.top

JS:   throw new Error("错误信息");
来源：http://cax.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://ixd.daria6918.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wia.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cwo.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dza.sxryk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sgw.jqgfzy.top

[H04] 自定义异常类型
来源：http://ezd.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://jyn.nanxinkj.top

PHP:  class MyError extends RuntimeException {}
来源：http://pch.ydzc1.top

JS:   class MyError extends Error {}
来源：http://vnt.jqgfzy.top

TS:   class MyError extends Error {}
来源：http://ezi.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://sfi.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tnl.sjlbkw.cn

Ruby: class MyError < StandardError; end
来源：http://ydp.cdnleiting.top

C#:   class MyException : Exception {}
来源：http://nxx.hesvh.cn

[H05] 捕获特定类型
来源：http://ccg.hywenlv.cn

Py:   except ValueError as e:
来源：http://hbd.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gzq.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://bga.xziqi.cn

TS:   if (e instanceof TypeError) {}
来源：http://rah.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://mmy.smart0.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vmy.cheryme.top

Ruby: rescue ArgumentError => e
来源：http://lwi.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xwp.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://iqm.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://zpb.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://goz.yfazqb.com

JS:   obj?.a?.b;  d ?? default
来源：http://qpq.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://emb.ydjk.org.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qmv.zhixingplan.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qay.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://edf.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://mwp.svipenyu.cn

[H07] 断言
来源：http://wvc.tanke756.top

Py:   assert x > 0, "必须为正"
来源：http://pfw.ehwqpu.com

PHP:  assert($x > 0);
来源：http://nso.ivvv.top

JS:   console.assert(x > 0);
来源：http://rwi.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://vxn.ywan-chungtsiang.top

Java: assert x > 0 : "必须为正";
来源：http://ooy.snrcjt.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rmv.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://twg.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://vjj.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://nmh.shanyushiyangtech.top

Py:   str(e);  traceback.format_exc()
来源：http://idt.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xlo.jiagoushi.top

JS:   e.message;  e.stack
来源：http://asc.xylfe.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qfh.guannengcc.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mww.daxiang520.top

Go:   err.Error()
来源：http://slf.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://flw.dianchejie.cn

C#:   e.Message;  e.StackTrace
来源：http://vgy.zhixingplan.top

[H09] 带错误码的异常
来源：http://xqh.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ypo.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://uwi.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://azq.yuanzhike.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vtg.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jwc.birdmap.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://irz.ydzc1.top

Ruby: raise MyError.new("fail", 500)
来源：http://wrp.yangfankeji.com

C#:   // 自定义异常类中加 Code 属性
来源：http://gjh.0kj1m.cn

[H10] 资源自动释放
来源：http://wid.hesvh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://crq.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://isn.yj202588.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zml.shangyingyoupin.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vwz.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://flr.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://pot.52xcode.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ami.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sqx.daria6918.cn

================================================================================
来源：http://gnb.shanyushiyangkeji.top

I. 正则表达式
来源：http://gxz.xylfe.cn

================================================================================
来源：http://gts.nanxuanxn.top

[I01] 判断是否匹配
来源：http://odf.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://awi.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zqq.kuanghao11.cn

JS:   /\d+/.test(s)
来源：http://ola.xziqi.cn

TS:   /\d+/.test(s)
来源：http://bxh.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kyq.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sqs.9152youxi.cn

Ruby: s.match?(/\d+/)
来源：http://iyp.hnxiangtu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://crj.gaohongyu789.top

[I02] 提取所有匹配
来源：http://aiq.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://xvd.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hch.dashuyun.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tka.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://cbf.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lcb.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://egx.gotoacloud.top

Ruby: s.scan(/\d+/)
来源：http://ksj.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kst.sxryk.cn

[I03] 提取捕获分组
来源：http://mru.yueranfly.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kom.jinyuanbaomall.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://piv.zhijiandao.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://grm.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tyy.xinyue.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tns.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ayo.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mkt.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://faw.gzhubu.top

[I04] 正则替换
来源：http://tbo.yuanzhike.top

Py:   re.sub(r"\d+", "#", s)
来源：http://owa.0kj1m.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://teo.xinyue.icu

JS:   s.replace(/\d+/g, "#")
来源：http://hzz.ydzc1.top

TS:   s.replace(/\d+/g, "#")
来源：http://rij.tanke756.top

Java: s.replaceAll("\\d+", "#")
来源：http://pyi.dianchejie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xjb.jianghu66.top

Ruby: s.gsub(/\d+/, "#")
来源：http://npu.yfazqb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ubs.gaohongyu789.top

[I05] 按正则拆分
来源：http://fyr.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://qsw.yj20258.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bgk.ivvv.top

JS:   s.split(/\s*,\s*/)
来源：http://oqe.hfpthk.cn

TS:   s.split(/\s*,\s*/)
来源：http://wah.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://dxa.yj20258888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jlw.ywan-chungtsiang.top

Ruby: s.split(/\s*,\s*/)
来源：http://xcj.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://alg.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yjy.sufxvd.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://imx.tarul.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sdd.xuetiantiany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jzb.gaohongyu789.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nxo.jlsjyb.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tam.fanxiaobao.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tgp.xingfuxueyuan.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ubb.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://etz.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://upb.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gvy.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nzy.ydjk.org.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://njd.hywenlv.cn

TS:   /error/gim
来源：http://mwy.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rel.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nom.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://ojo.pengpengdd.cyou

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://boe.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://tnh.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qrj.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nsg.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iwe.iojbl.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hif.ydjk.org.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wtj.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kio.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://akc.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ids.shuidangran.top

================================================================================
来源：http://mwy.havefunace.top

J. 日期与时间
来源：http://jwe.shanyushiyangtech.top

================================================================================
来源：http://aft.nanxuanxn.top

[J01] 获取当前时间
来源：http://xkg.guowangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://eiy.sufxvd.cn


<!-- 参考信息 -->