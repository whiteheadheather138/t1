代发 wailian999

Py:   class Admin(User): pass
来源：http://aso.zhijiandao.cn

PHP:  class Admin extends User {}
来源：http://jen.sweek.top

JS:   class Admin extends User {}
来源：http://tcb.hywenlv.cn

TS:   class Admin extends User {}
来源：http://jxp.zdqjudy.top

Java: class Admin extends User {}
来源：http://ttl.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jcj.cashguo.top

Ruby: class Admin < User; end
来源：http://hpi.fktsv.cn

C#:   class Admin : User {}
来源：http://yjf.ctjpmb.com

[G06] 重写方法
来源：http://cxq.yongpay.top

Py:   def greet(self): return "admin"
来源：http://qbb.cqqwz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eko.9152youxi.cn

JS:   greet() { return "admin"; }
来源：http://jrg.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://rxq.jqgfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://aqf.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zoy.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://cce.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://loh.shuidangran.top

[G07] 调用父类方法
来源：http://une.jqgfzy.top

Py:   super().greet()
来源：http://mlo.0kj1m.cn

PHP:  parent::greet();
来源：http://vse.fzhhl.top

JS:   super.greet();
来源：http://avn.zhiwuduotai.top

TS:   super.greet();
来源：http://yaq.nanxinkj.top

Java: super.greet();
来源：http://njz.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ihb.svipenyu.cn

Ruby: super
来源：http://cki.pengpengdd.cyou

C#:   base.Greet();
来源：http://ald.daria6918.cn

[G08] 静态方法与属性
来源：http://kbb.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lvv.sweek.top

PHP:  public static function f() {}
来源：http://uab.zhixingplan.top

JS:   static f() {}
来源：http://hgg.fehbvm.com

TS:   static f(): void {}
来源：http://uca.nanxinkj.top

Java: static void f() {}
来源：http://fit.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mxo.cashguo.top

Ruby: def self.f; end
来源：http://kxd.52xcode.cn

C#:   public static void F() {}
来源：http://saw.jlsjyb.cn

[G09] 接口 / 抽象类
来源：http://lmt.jqgfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://pat.wangshuangyany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://weh.bbcook.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fyz.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://idw.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://rht.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://ccq.c1oappe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wfo.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://jrt.zhongyouzk.top

[G10] 访问控制
来源：http://hef.shangyingyoupin.top

Py:   约定 _protected / __private（不强制）
来源：http://efr.jqgfzy.top

PHP:  public / protected / private
来源：http://iyd.bbcook.cn

JS:   #private 字段；其余公开
来源：http://wjt.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://kvk.haohaochexian.top

Java: public / protected / private / 默认包级
来源：http://slp.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nwq.sjlbkw.cn

Ruby: public / protected / private
来源：http://cwv.aizwys.cn

C#:   public / protected / private / internal
来源：http://brs.fktsv.cn

[G11] getter / setter
来源：http://opd.nanxuanxn.top

Py:   @property 与 @x.setter
来源：http://fxf.fktsv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ntw.bjfxy.top

JS:   get name() { return this._name; }
来源：http://tpj.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://qla.vehdjk.com

Java: public String getName() { return name; }
来源：http://quq.yj20258.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kka.0kj1m.cn

Ruby: attr_accessor :name
来源：http://bog.yvedp.cn

C#:   public string Name { get; set; }
来源：http://bot.zdbjq.cn

[G12] 对象转字符串
来源：http://ksj.yonumen.top

Py:   def __str__(self): return self.name
来源：http://mkx.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://spn.ehwqpu.com

JS:   toString() { return this.name; }
来源：http://rtm.yanxiufei.cn

TS:   toString(): string { return this.name; }
来源：http://lru.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://ysz.hywenlv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ufg.ybcxt.top

Ruby: def to_s; @name; end
来源：http://dmo.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://xtq.jinyuanbaomall.cn

[G13] 判断对象类型
来源：http://sbo.xuetiantiany.cn

Py:   isinstance(u, User)
来源：http://yno.jiagoushi.top

PHP:  $u instanceof User
来源：http://ccm.ydjk.org.cn

JS:   u instanceof User
来源：http://hqu.nwbrower.top

TS:   u instanceof User
来源：http://twy.hnqzz.top

Java: u instanceof User
来源：http://fmt.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://doz.zhengqikj.top

Ruby: u.is_a?(User)
来源：http://vhp.hcnkem.com

C#:   u is User
来源：http://cpb.daxiang520.top

[G14] 数据类 / record
来源：http://qni.aibaodan.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rlf.zhongyouzk.top

PHP:  // 用 readonly 属性模拟
来源：http://cxm.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lga.yueranfly.top

TS:   type User = { name: string; age: number };
来源：http://wdy.daria6918.cn

Java: record User(String name, int age) {}
来源：http://wfd.zhoulong.xyz

Go:   type User struct { Name string; Age int }
来源：http://pex.cdnleiting.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yai.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://dza.zhoulong.xyz

[G15] 枚举
来源：http://hkb.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ukn.daria6918.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://snf.jinghuilouyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gli.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ddk.jinyuanbaomall.cn

Java: enum Color { RED, GREEN }
来源：http://bup.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qpz.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://mfv.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dmg.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://ogv.cashguo.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oqq.bbcook.cn

PHP:  get_object_vars($obj);
来源：http://mnm.daria6918.cn

JS:   Object.entries(obj)
来源：http://jna.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://xoo.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bxn.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://yfg.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://wqp.uphjek.com

C#:   // 用反射或 System.Text.Json
来源：http://mtg.sxryk.cn

================================================================================
来源：http://cmm.aibaodan.cn

H. 异常与错误处理
来源：http://oed.fzhhl.top

================================================================================
来源：http://sto.haohaochexian.top

[H01] try / catch 基础
来源：http://udv.fktsv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wzj.guannengcc.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qjt.bbcook.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jjh.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ims.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pxl.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ewb.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cqb.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bao.sxryk.cn

[H02] finally / ensure 收尾
来源：http://phj.hcnkem.com

Py:   try: f()⏎finally: cleanup()
来源：http://mba.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jww.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dic.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://psq.feifeiyinyue.top

Java: try { f(); } finally { cleanup(); }
来源：http://lht.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://aie.jqgfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zbh.zhengqikj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hto.snrcjt.cn

[H03] 主动抛出异常
来源：http://kad.redwolf501.top

Py:   raise ValueError("错误信息")
来源：http://iak.316326.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://koy.guannengcc.top

JS:   throw new Error("错误信息");
来源：http://yfx.sufxvd.cn

TS:   throw new Error("错误信息");
来源：http://gcb.yj202588.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hsx.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ghm.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://giq.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://peq.tian-w.cn

[H04] 自定义异常类型
来源：http://nlw.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://gvm.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uci.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://qnz.jlsjyb.cn

TS:   class MyError extends Error {}
来源：http://hgf.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://nnq.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ufv.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://mbr.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://kyb.zhongyouzk.top

[H05] 捕获特定类型
来源：http://rek.zhengqikj.top

Py:   except ValueError as e:
来源：http://jzd.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vec.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://fvx.jinghuilouyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://qhc.tian-w.cn

Java: catch (IOException | SQLException e) {}
来源：http://xav.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uuv.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://pgx.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mcn.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://atj.pycfn.com

Py:   value = d.get("k") or default
来源：http://sna.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wdy.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://jji.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bnb.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pva.sxryk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vff.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://nyn.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://gbj.xuetiantiany.cn

[H07] 断言
来源：http://gqc.vehdjk.com

Py:   assert x > 0, "必须为正"
来源：http://lce.ctjpmb.com

PHP:  assert($x > 0);
来源：http://guq.zycfv.cn

JS:   console.assert(x > 0);
来源：http://bme.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://clp.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://emc.zhongyouzk.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xfp.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mfq.svipenyu.cn

C#:   Debug.Assert(x > 0);
来源：http://mgm.ehwqpu.com

[H08] 获取错误信息与堆栈
来源：http://eda.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://xjw.bbcook.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vcp.shzxlz.cn

JS:   e.message;  e.stack
来源：http://xqm.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bwg.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://alc.yanxiufei.cn

Go:   err.Error()
来源：http://zbt.yongpay.top

Ruby: e.message;  e.backtrace
来源：http://zkm.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://zlz.jinqigfzy.top

[H09] 带错误码的异常
来源：http://skh.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ouz.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ahc.zycfv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wyu.yj20258888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yno.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tup.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uoh.hnxiangtu.top

Ruby: raise MyError.new("fail", 500)
来源：http://fet.jinyuanbaomall.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fte.9152youxi.cn

[H10] 资源自动释放
来源：http://qcg.yanxiufei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://woc.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://axu.jiagoushi.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ufr.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ybh.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nap.gaohongyu789.top

Go:   defer f.Close()
来源：http://eha.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wsq.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bpz.yueranfly.top

================================================================================
来源：http://yem.yj20258.top

I. 正则表达式
来源：http://dfa.xingfuxueyuan.xyz

================================================================================
来源：http://spo.tarul.cn

[I01] 判断是否匹配
来源：http://kub.feifeiyinyue.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://weo.shuidangran.top

PHP:  preg_match('/\d+/', $s);
来源：http://jvg.sufxvd.cn

JS:   /\d+/.test(s)
来源：http://jan.nanxuanxn.top

TS:   /\d+/.test(s)
来源：http://nll.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vyz.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hhz.pycfn.com

Ruby: s.match?(/\d+/)
来源：http://ntw.kuanghao11.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zge.tianlin.xyz

[I02] 提取所有匹配
来源：http://erz.pengpengdd.cyou

Py:   re.findall(r"\d+", s)
来源：http://tey.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mbr.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ycr.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://mka.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wcc.hnqzz.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fyy.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://shw.fanxiaobao.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sdm.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://jqs.ehwqpu.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://axt.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qlc.birdmap.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sek.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eev.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://itc.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ado.jqgufenzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yij.hcnkem.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tkq.kuanghao11.cn

[I04] 正则替换
来源：http://itz.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://imy.tian-w.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rkr.cqqwz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://coh.tanke756.top

TS:   s.replace(/\d+/g, "#")
来源：http://jpo.bjfxy.top

Java: s.replaceAll("\\d+", "#")
来源：http://bll.gaohongyu789.top

Go:   re.ReplaceAllString(s, "#")
来源：http://clw.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://njv.shuidangran.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rlf.xylfe.cn

[I05] 按正则拆分
来源：http://kbm.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://etj.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fjr.chenjidiqi.icu

JS:   s.split(/\s*,\s*/)
来源：http://cqg.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://vwe.cashguo.top

Java: s.split("\\s*,\\s*")
来源：http://kdm.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eus.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://gtg.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jjl.fktsv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kwu.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oiw.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ira.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qqm.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qis.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aqq.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qxg.zhongyouzk.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ext.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gwh.9152youxi.cn

[I07] 忽略大小写与多行模式
来源：http://jgo.jianghu66.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://htr.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://knp.pycfn.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kci.uphjek.com

TS:   /error/gim
来源：http://mfi.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://apf.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gww.shanyushiyangtech.top

Ruby: s.scan(/error/i)
来源：http://fsg.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zvu.wangdashe.top

[I08] 贪婪与非贪婪匹配
来源：http://vmz.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ggp.hfpthk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kwt.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qmr.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jjk.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://elb.pengpengdd.cyou

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vjb.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mlw.yangfankeji.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bcv.tanke756.top

================================================================================
来源：http://dyi.tianlin.xyz

J. 日期与时间
来源：http://gxb.meibo888.top

================================================================================
来源：http://cev.zhongyouzk.top

[J01] 获取当前时间
来源：http://dtj.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nwp.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ags.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://aqq.yj202588.top

TS:   new Date();  Date.now()
来源：http://irk.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://vho.hnxiangtu.top

Go:   time.Now()
来源：http://fel.hnqzz.top

Ruby: Time.now
来源：http://cku.redwolf501.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uzv.zdqjudy.top

[J02] 格式化输出
来源：http://nww.nanxinkj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ojw.yvedp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nyz.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pwj.jqgufenzy.top

TS:   d.toISOString()
来源：http://rjb.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ehn.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hxk.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://olu.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qwt.pycfn.com

[J03] 字符串解析为日期
来源：http://cpc.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://btt.gotoacloud.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tyd.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://usb.fehbvm.com


<!-- 参考信息 -->