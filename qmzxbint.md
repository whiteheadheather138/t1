代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://fni.jinyuanbaomall.cn

JS:   greet() { return this.name; }
来源：http://ycq.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://nwk.yanxiufei.cn

Java: String greet() { return name; }
来源：http://kpx.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ooa.tianlin.xyz

Ruby: def greet; @name; end
来源：http://obe.guannengcc.top

C#:   public string Greet() => Name;
来源：http://skx.9152youxi.cn

[G05] 继承
来源：http://pqk.ydjk.org.cn

Py:   class Admin(User): pass
来源：http://szc.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://oas.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://lyz.cdnleiting.top

TS:   class Admin extends User {}
来源：http://qva.sxryk.cn

Java: class Admin extends User {}
来源：http://yoc.zhongyouzk.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://juc.zhaomingkeji.xyz

Ruby: class Admin < User; end
来源：http://bdd.shzxlz.cn

C#:   class Admin : User {}
来源：http://tpz.gaohongyu789.top

[G06] 重写方法
来源：http://aqn.hfpthk.cn

Py:   def greet(self): return "admin"
来源：http://spm.dianchejie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oqi.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://uuy.tarul.cn

TS:   greet(): string { return "admin"; }
来源：http://yyw.quarkkingdee.top

Java: @Override String greet() { return "admin"; }
来源：http://wcd.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wqh.xuanzx.com

Ruby: def greet; "admin"; end
来源：http://qnn.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://vsv.ybcxt.top

[G07] 调用父类方法
来源：http://vfk.shangyingyoupin.top

Py:   super().greet()
来源：http://vkp.fanxiaobao.xyz

PHP:  parent::greet();
来源：http://vzh.meibo888.top

JS:   super.greet();
来源：http://tgr.gogol.net.cn

TS:   super.greet();
来源：http://xwu.jlsjyb.cn

Java: super.greet();
来源：http://rfh.hywenlv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ytu.iojbl.cn

Ruby: super
来源：http://uxr.zhijiandao.cn

C#:   base.Greet();
来源：http://buy.shuidangran.top

[G08] 静态方法与属性
来源：http://oei.vehdjk.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dxr.kuanghao11.cn

PHP:  public static function f() {}
来源：http://szf.zhixingplan.top

JS:   static f() {}
来源：http://trn.tarul.cn

TS:   static f(): void {}
来源：http://qcb.zhengqikj.top

Java: static void f() {}
来源：http://lpx.jinyuanbaomall.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ffh.yvedp.cn

Ruby: def self.f; end
来源：http://ckn.shzxlz.cn

C#:   public static void F() {}
来源：http://wet.epnwcf.com

[G09] 接口 / 抽象类
来源：http://twr.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://uqd.bjfxy.top

PHP:  interface Shape { public function area(): float; }
来源：http://zoc.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dfg.nanxinkj.top

TS:   interface Shape { area(): number; }
来源：http://nzr.bjfxy.top

Java: interface Shape { double area(); }
来源：http://lyy.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://mto.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lqe.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://jie.yongpay.top

[G10] 访问控制
来源：http://hbv.zhaomingkeji.xyz

Py:   约定 _protected / __private（不强制）
来源：http://rgg.hcnkem.com

PHP:  public / protected / private
来源：http://dnt.svipenyu.cn

JS:   #private 字段；其余公开
来源：http://kby.zhiwuduotai.top

TS:   public / protected / private
来源：http://unt.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://moi.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://wbn.sweek.top

Ruby: public / protected / private
来源：http://vcl.shangyingyoupin.top

C#:   public / protected / private / internal
来源：http://ldn.hcnkem.com

[G11] getter / setter
来源：http://yxc.tanke756.top

Py:   @property 与 @x.setter
来源：http://bdu.yj20258.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fbr.hywenlv.cn

JS:   get name() { return this._name; }
来源：http://kqx.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://ipd.shanyushiyangkeji.top

Java: public String getName() { return name; }
来源：http://fbg.smart0.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://seb.fehbvm.com

Ruby: attr_accessor :name
来源：http://fll.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://bfr.sufxvd.cn

[G12] 对象转字符串
来源：http://whu.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://zvc.meibo888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zrh.zycfv.cn

JS:   toString() { return this.name; }
来源：http://flg.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://bng.tianlin.xyz

Java: @Override public String toString() { return name; }
来源：http://umf.chenjidiqi.icu

Go:   func (u User) String() string { return u.Name }
来源：http://byn.andypj.xyz

Ruby: def to_s; @name; end
来源：http://ecr.hongshengwenyu.top

C#:   public override string ToString() => Name;
来源：http://pzv.fzhhl.top

[G13] 判断对象类型
来源：http://cbd.ivvv.top

Py:   isinstance(u, User)
来源：http://biz.jyoumei.cn

PHP:  $u instanceof User
来源：http://ppf.redwolf501.top

JS:   u instanceof User
来源：http://clz.jianghu66.top

TS:   u instanceof User
来源：http://lcb.yongpay.top

Java: u instanceof User
来源：http://qpl.nanxinkj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fgg.feifeiyinyue.top

Ruby: u.is_a?(User)
来源：http://dpz.cqqwz.cn

C#:   u is User
来源：http://wzs.smart0.xyz

[G14] 数据类 / record
来源：http://qil.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lzz.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://bmp.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://afs.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://tan.zhengqikj.top

Java: record User(String name, int age) {}
来源：http://ifn.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://buw.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mur.fengsongda.top

C#:   record User(string Name, int Age);
来源：http://prd.yangfankeji.com

[G15] 枚举
来源：http://rqv.shangyingyoupin.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://whb.vqdsnc.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dlr.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xka.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://spr.yvedp.cn

Java: enum Color { RED, GREEN }
来源：http://amt.zdbjq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qsf.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://jbj.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fkx.tarul.cn

[G16] 对象转数组 / 字典
来源：http://dxj.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://naf.jinghuilouyu.cn

PHP:  get_object_vars($obj);
来源：http://zse.9152youxi.cn

JS:   Object.entries(obj)
来源：http://dbi.shanyushiyangkeji.top

TS:   Object.entries(obj)
来源：http://tai.guowangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kss.shangyingyoupin.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bxg.ctjpmb.com

Ruby: obj.instance_variables
来源：http://ivs.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://lol.yangfankeji.com

================================================================================
来源：http://ibc.vqdsnc.cn

H. 异常与错误处理
来源：http://bzi.hnxiangtu.top

================================================================================
来源：http://acw.nwbrower.top

[H01] try / catch 基础
来源：http://rox.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qfi.daria6918.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yqs.ywan-chungtsiang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rww.meibo888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ggp.c1oappe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kqa.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kqd.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uwl.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hop.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://ljb.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://dwx.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://kby.tian-w.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bzz.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://clv.ehwqpu.com

Java: try { f(); } finally { cleanup(); }
来源：http://dwf.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wnt.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jqn.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xcv.yj202588.top

[H03] 主动抛出异常
来源：http://mng.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://zxr.cashguo.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sok.chenjidiqi.icu

JS:   throw new Error("错误信息");
来源：http://yli.ivvv.top

TS:   throw new Error("错误信息");
来源：http://fad.hnxiangtu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fyp.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jka.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mae.jinqigufen.top

C#:   throw new ArgumentException("错误信息");
来源：http://jyb.gaohongyu789.top

[H04] 自定义异常类型
来源：http://xiy.jianghu66.top

Py:   class MyError(Exception): pass
来源：http://vku.hongshengwenyu.top

PHP:  class MyError extends RuntimeException {}
来源：http://vfn.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://xlx.ybcxt.top

TS:   class MyError extends Error {}
来源：http://oly.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://ztf.chenlongwang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pbu.sxryk.cn

Ruby: class MyError < StandardError; end
来源：http://hfn.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://kuu.nanxuanxn.top

[H05] 捕获特定类型
来源：http://bnw.yuanzhike.top

Py:   except ValueError as e:
来源：http://mgp.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rtf.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://and.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://syf.bbcook.cn

Java: catch (IOException | SQLException e) {}
来源：http://mpe.0kj1m.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ork.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://nmb.hysaishi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wsv.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://xrh.fehbvm.com

Py:   value = d.get("k") or default
来源：http://apq.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://onk.tian-w.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hej.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ogf.nanxinkj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dqn.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qls.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://jpm.nwbrower.top

C#:   obj?.A?.B ?? default
来源：http://unb.hammf.cn

[H07] 断言
来源：http://yhe.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://utb.yueranfly.top

PHP:  assert($x > 0);
来源：http://zrx.ydzc1.top

JS:   console.assert(x > 0);
来源：http://rwm.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://ceh.jinghuilouyu.cn

Java: assert x > 0 : "必须为正";
来源：http://pdv.zycfv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wnu.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://uqr.pengpengdd.cyou

C#:   Debug.Assert(x > 0);
来源：http://hbg.yuxming.cn

[H08] 获取错误信息与堆栈
来源：http://hvb.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://fzb.shzxlz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tmn.jiagoushi.top

JS:   e.message;  e.stack
来源：http://fuc.hnqzz.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ish.jlsjyb.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mie.jqgufenzy.top

Go:   err.Error()
来源：http://qjn.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://nkc.sysykeji.top

C#:   e.Message;  e.StackTrace
来源：http://dnz.daxiang520.top

[H09] 带错误码的异常
来源：http://yps.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nrb.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mmw.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bmn.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nui.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hck.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://teb.jlsjyb.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bqd.gogol.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wlo.gogol.net.cn

[H10] 资源自动释放
来源：http://kvh.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://dwk.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ltx.ydzc1.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ish.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tyy.cqqwz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xtt.nanxinkj.top

Go:   defer f.Close()
来源：http://cfq.ivvv.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zfk.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://shi.gogol.net.cn

================================================================================
来源：http://aem.haohaochexian.top

I. 正则表达式
来源：http://zvh.guowangkeji.top

================================================================================
来源：http://zhv.guowangkeji.top

[I01] 判断是否匹配
来源：http://aom.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wbr.sufxvd.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sol.52xcode.cn

JS:   /\d+/.test(s)
来源：http://nwx.hnqzz.top

TS:   /\d+/.test(s)
来源：http://cza.sweek.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tbs.andypj.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qct.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://zqk.jyoumei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hgw.yj202588.top

[I02] 提取所有匹配
来源：http://bic.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://ypi.yangfankeji.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ytg.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tyj.pycfn.com

TS:   s.match(/\d+/g)
来源：http://fpd.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://min.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fat.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://man.zhixingplan.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rpf.andypj.xyz

[I03] 提取捕获分组
来源：http://ccq.fktsv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pfk.xylfe.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xoa.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pqd.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vjl.ybcxt.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iet.daxiang520.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wpg.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://idk.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fjb.sxryk.cn

[I04] 正则替换
来源：http://qug.52xcode.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zgi.hongshengwenyu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mby.xziqi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wqh.tianlin.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://zwk.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://kol.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gji.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ogq.gogol.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://igv.c1oappe.top

[I05] 按正则拆分
来源：http://cdu.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://bnr.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xaj.hfpthk.cn

JS:   s.split(/\s*,\s*/)
来源：http://cnt.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://hzw.yanxiufei.cn

Java: s.split("\\s*,\\s*")
来源：http://sbv.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rgb.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gcq.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ryp.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iom.jinyuanbaomall.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pbt.ybcxt.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cia.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ded.ivvv.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://prz.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pgu.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hkd.ctjpmb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ben.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tgw.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://lxy.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hyq.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xru.cashguo.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rnb.cucudq.cn

TS:   /error/gim
来源：http://lrj.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ezl.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gnn.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://dub.316326.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lrn.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://foc.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rnc.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://boc.nanxuanxn.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nks.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://csn.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ptx.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gtz.zhaomingkeji.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hjt.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dml.meibo888.top

================================================================================
来源：http://iit.jinyuanbaomall.cn

J. 日期与时间
来源：http://jtz.ydjk.org.cn

================================================================================
来源：http://ngc.yanxiufei.cn

[J01] 获取当前时间
来源：http://ajx.hfpthk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bci.haohaochexian.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uuw.chenlongwang.top

JS:   new Date();  Date.now()
来源：http://efd.cucudq.cn

TS:   new Date();  Date.now()
来源：http://gyz.nanxuanxn.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pms.jinyuanbaomall.cn

Go:   time.Now()
来源：http://kze.shanyushiyangtech.top

Ruby: Time.now
来源：http://nyn.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://edd.9152youxi.cn

[J02] 格式化输出
来源：http://pjb.gzhubu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://agg.chenlongwang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oqj.shuidangran.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qvj.yfazqb.com

TS:   d.toISOString()
来源：http://cwy.hcnkem.com


<!-- 参考信息 -->