代发 wailian999

Ruby: @name = "x"
来源：http://mpl.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ayc.daria6918.cn

[G04] 定义方法
来源：http://yzp.xuanzx.com

Py:   def greet(self): return self.name
来源：http://hcn.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fmp.zdqjudy.top

JS:   greet() { return this.name; }
来源：http://hkq.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://yta.zhijiandao.cn

Java: String greet() { return name; }
来源：http://mmx.yonumen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ngd.yfazqb.com

Ruby: def greet; @name; end
来源：http://cib.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://ppk.shzxlz.cn

[G05] 继承
来源：http://tug.jinqigufen.top

Py:   class Admin(User): pass
来源：http://mqu.iojbl.cn

PHP:  class Admin extends User {}
来源：http://zlk.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://jzb.hammf.cn

TS:   class Admin extends User {}
来源：http://wiu.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://nre.hnxiangtu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yll.dashuyun.cn

Ruby: class Admin < User; end
来源：http://lnq.epnwcf.com

C#:   class Admin : User {}
来源：http://ehd.zhiwuduotai.top

[G06] 重写方法
来源：http://qss.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://qzu.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://kov.yangfankeji.com

JS:   greet() { return "admin"; }
来源：http://tdk.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://tzi.bjfxy.top

Java: @Override String greet() { return "admin"; }
来源：http://yxl.yanxiufei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rov.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://avh.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://zpc.jyoumei.cn

[G07] 调用父类方法
来源：http://ztr.zhongyouzk.top

Py:   super().greet()
来源：http://sje.yj202588.top

PHP:  parent::greet();
来源：http://rvz.gaohongyu789.top

JS:   super.greet();
来源：http://scu.xylfe.cn

TS:   super.greet();
来源：http://egq.yuxming.cn

Java: super.greet();
来源：http://yqi.gotoacloud.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gxi.xziqi.cn

Ruby: super
来源：http://rgo.vehdjk.com

C#:   base.Greet();
来源：http://swn.tian-w.cn

[G08] 静态方法与属性
来源：http://xik.yj20258888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://klq.xingfuxueyuan.xyz

PHP:  public static function f() {}
来源：http://uum.tianlin.xyz

JS:   static f() {}
来源：http://hoy.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://vlp.redwolf501.top

Java: static void f() {}
来源：http://cni.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://abi.jianghu66.top

Ruby: def self.f; end
来源：http://goq.uphjek.com

C#:   public static void F() {}
来源：http://dop.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://scw.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://wde.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://nou.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bqd.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://imh.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://xga.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://ege.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wxm.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://wyo.feifeiyinyue.top

[G10] 访问控制
来源：http://wqs.52xcode.cn

Py:   约定 _protected / __private（不强制）
来源：http://gnt.haohaochexian.top

PHP:  public / protected / private
来源：http://vux.sjlbkw.cn

JS:   #private 字段；其余公开
来源：http://nvx.xylfe.cn

TS:   public / protected / private
来源：http://iyo.jinqigufen.top

Java: public / protected / private / 默认包级
来源：http://ypt.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vkf.jlsjyb.cn

Ruby: public / protected / private
来源：http://msk.c1oappe.top

C#:   public / protected / private / internal
来源：http://fvb.tarul.cn

[G11] getter / setter
来源：http://adw.tian-w.cn

Py:   @property 与 @x.setter
来源：http://hta.ydjk.org.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://civ.xuanzx.com

JS:   get name() { return this._name; }
来源：http://cxh.hywenlv.cn

TS:   get name(): string { return this._name; }
来源：http://sfq.9152youxi.cn

Java: public String getName() { return name; }
来源：http://bip.jqgufenzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dum.c1oappe.top

Ruby: attr_accessor :name
来源：http://szy.fanxiaobao.xyz

C#:   public string Name { get; set; }
来源：http://fki.xziqi.cn

[G12] 对象转字符串
来源：http://tfo.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://jzn.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://zrp.cheryme.top

JS:   toString() { return this.name; }
来源：http://ulq.yanxiufei.cn

TS:   toString(): string { return this.name; }
来源：http://zhz.cqqwz.cn

Java: @Override public String toString() { return name; }
来源：http://ygs.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vkc.jyoumei.cn

Ruby: def to_s; @name; end
来源：http://fbq.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://zxd.dashuyun.cn

[G13] 判断对象类型
来源：http://ocr.smart0.xyz

Py:   isinstance(u, User)
来源：http://vhp.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://gfj.shzxlz.cn

JS:   u instanceof User
来源：http://pln.sweek.top

TS:   u instanceof User
来源：http://duo.yuanzhike.top

Java: u instanceof User
来源：http://vxt.gogol.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://egf.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://tvh.jinghuilouyu.cn

C#:   u is User
来源：http://cip.yuxming.cn

[G14] 数据类 / record
来源：http://evh.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vgm.hfpthk.cn

PHP:  // 用 readonly 属性模拟
来源：http://heh.zhoulong.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://oiw.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://zvn.c1oappe.top

Java: record User(String name, int age) {}
来源：http://syq.shanyushiyangtech.top

Go:   type User struct { Name string; Age int }
来源：http://umf.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://heq.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://ipw.gogol.net.cn

[G15] 枚举
来源：http://pjq.cdnleiting.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cqm.sjlbkw.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://joj.gzhubu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iew.yongpay.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nhh.shanyushiyangkeji.top

Java: enum Color { RED, GREEN }
来源：http://ddy.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kgy.yuxming.cn

Ruby: Color = %i[red green].freeze
来源：http://jck.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rxr.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://vuf.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kse.feifeiyinyue.top

PHP:  get_object_vars($obj);
来源：http://gcg.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://eiv.yj20258.top

TS:   Object.entries(obj)
来源：http://wmt.ydzc1.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ury.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jgj.xziqi.cn

Ruby: obj.instance_variables
来源：http://eoq.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://aaw.hnxiangtu.top

================================================================================
来源：http://vjh.xylfe.cn

H. 异常与错误处理
来源：http://vcs.0kj1m.cn

================================================================================
来源：http://tvv.hongshengwenyu.top

[H01] try / catch 基础
来源：http://lsu.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wci.snrcjt.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mjr.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nhj.bbcook.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oby.zycfv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nju.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sbo.yuanzhike.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://irr.chenjidiqi.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kot.fzhhl.top

[H02] finally / ensure 收尾
来源：http://dyr.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://puz.shanyushiyangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vkd.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://crs.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qap.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://nfc.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://izl.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://juu.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uyp.zycfv.cn

[H03] 主动抛出异常
来源：http://nhx.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://fnu.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mqg.sxryk.cn

JS:   throw new Error("错误信息");
来源：http://phi.hnxiangtu.top

TS:   throw new Error("错误信息");
来源：http://zkn.0kj1m.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sef.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cbu.sufxvd.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://djr.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://nsl.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://lqi.ydzc1.top

Py:   class MyError(Exception): pass
来源：http://wxd.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://wvf.yongpay.top

JS:   class MyError extends Error {}
来源：http://odq.tianlin.xyz

TS:   class MyError extends Error {}
来源：http://ztz.pycfn.com

Java: class MyException extends RuntimeException {}
来源：http://uld.jlsjyb.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vih.yj20258888.top

Ruby: class MyError < StandardError; end
来源：http://syc.nanxuanxn.top

C#:   class MyException : Exception {}
来源：http://sam.snrcjt.cn

[H05] 捕获特定类型
来源：http://tip.yueranfly.top

Py:   except ValueError as e:
来源：http://avh.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jow.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://jex.fanxiaobao.xyz

TS:   if (e instanceof TypeError) {}
来源：http://loj.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://oza.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xnd.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://bov.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yza.zhoulong.xyz

[H06] 可选值 / 空值安全访问
来源：http://lhf.sufxvd.cn

Py:   value = d.get("k") or default
来源：http://gcg.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://ewy.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xwd.bjfxy.top

TS:   obj?.a?.b;  d ?? default
来源：http://hke.shangyingyoupin.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uji.hnxiangtu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zvs.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://fqb.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://wko.shzxlz.cn

[H07] 断言
来源：http://fst.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://fyt.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://ngh.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://zjs.xingfuxueyuan.xyz

TS:   console.assert(x > 0);
来源：http://ewm.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://gtv.fzhhl.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qsh.yueranfly.top

Ruby: raise "必须为正" unless x > 0
来源：http://krt.jiagoushi.top

C#:   Debug.Assert(x > 0);
来源：http://kok.aizwys.cn

[H08] 获取错误信息与堆栈
来源：http://gpq.chenjidiqi.icu

Py:   str(e);  traceback.format_exc()
来源：http://asm.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://miz.gaohongyu789.top

JS:   e.message;  e.stack
来源：http://lek.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sjm.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tmc.epnwcf.com

Go:   err.Error()
来源：http://gnh.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://cgc.dashuyun.cn

C#:   e.Message;  e.StackTrace
来源：http://hkx.jlsjyb.cn

[H09] 带错误码的异常
来源：http://bvx.andypj.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ari.ivvv.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mqh.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zmf.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cot.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wvl.wangdashe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pku.gogol.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zqs.jinqigfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xey.birdmap.top

[H10] 资源自动释放
来源：http://zdo.jinqigfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://drc.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://znl.c1oappe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uhc.redwolf501.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nrw.jinghuilouyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ldf.haohaochexian.top

Go:   defer f.Close()
来源：http://sac.yuxming.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yhd.gogol.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nvq.tarul.cn

================================================================================
来源：http://mfw.vehdjk.com

I. 正则表达式
来源：http://jzg.sweek.top

================================================================================
来源：http://tes.c1oappe.top

[I01] 判断是否匹配
来源：http://fow.cdnleiting.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hwl.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://luw.nanxinkj.top

JS:   /\d+/.test(s)
来源：http://dsm.cheryme.top

TS:   /\d+/.test(s)
来源：http://wdx.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vya.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xyj.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://hej.havefunace.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jqj.gotoacloud.top

[I02] 提取所有匹配
来源：http://pop.ywan-chungtsiang.top

Py:   re.findall(r"\d+", s)
来源：http://kkj.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pbq.feifeiyinyue.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pnr.yueranfly.top

TS:   s.match(/\d+/g)
来源：http://szy.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jdt.ybcxt.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://msr.sufxvd.cn

Ruby: s.scan(/\d+/)
来源：http://mvh.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lpe.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://hih.wangshuangyany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mxe.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nac.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hlb.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xsu.ivvv.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ymr.shzxlz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fod.tarul.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xzc.zhaomingkeji.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nzf.hesvh.cn

[I04] 正则替换
来源：http://qmg.nwbrower.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mfm.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qhx.jinyuanbaomall.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ghs.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yhr.tanke756.top

Java: s.replaceAll("\\d+", "#")
来源：http://mho.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://olp.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pvn.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xxi.meibo888.top

[I05] 按正则拆分
来源：http://zwv.xuetiantiany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ebx.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jru.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://clq.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://oce.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://ywh.sweek.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lvd.ppjwa.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qav.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gel.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ykj.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rmw.ybcxt.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gmc.meibo888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uvs.yj20258888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mag.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://epv.daxiang520.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aey.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qfj.sysykeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kfq.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://dap.hongshengwenyu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ant.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fyh.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bpc.hfpthk.cn

TS:   /error/gim
来源：http://rac.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://prc.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tfn.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://tsk.xuanzx.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qwh.svipenyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://gvp.guannengcc.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pco.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oas.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wji.yj20258888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bdf.yangfankeji.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ocr.jiagoushi.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nbh.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yek.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gri.sysykeji.top

================================================================================
来源：http://bxg.tian-w.cn

J. 日期与时间
来源：http://bir.feifeiyinyue.top

================================================================================
来源：http://exx.chenlongwang.top

[J01] 获取当前时间
来源：http://ubf.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tfp.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dnw.bbcook.cn

JS:   new Date();  Date.now()
来源：http://fgw.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://dfs.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uqr.redwolf501.top

Go:   time.Now()
来源：http://gkk.vqdsnc.cn

Ruby: Time.now
来源：http://bfj.yj202588.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ynj.jqgfzy.top

[J02] 格式化输出
来源：http://zud.dianchejie.cn


<!-- 参考信息 -->