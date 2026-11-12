代发 wailian999

Java: class Admin extends User {}
来源：http://acs.havefunace.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ntg.gotoacloud.top

Ruby: class Admin < User; end
来源：http://vcf.ydzc1.top

C#:   class Admin : User {}
来源：http://hfl.xziqi.cn

[G06] 重写方法
来源：http://ikb.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://mrh.sysykeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yno.yj202588.top

JS:   greet() { return "admin"; }
来源：http://cxl.fzhhl.top

TS:   greet(): string { return "admin"; }
来源：http://wjb.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://dgn.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ipb.wangdashe.top

Ruby: def greet; "admin"; end
来源：http://eos.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://yjg.zhoulong.xyz

[G07] 调用父类方法
来源：http://gsn.snrcjt.cn

Py:   super().greet()
来源：http://wef.xuetiantiany.cn

PHP:  parent::greet();
来源：http://ynd.sjlbkw.cn

JS:   super.greet();
来源：http://ylr.nanxuanxn.top

TS:   super.greet();
来源：http://fxs.meibo888.top

Java: super.greet();
来源：http://zqp.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vfd.smart0.xyz

Ruby: super
来源：http://qvi.havefunace.top

C#:   base.Greet();
来源：http://fbn.yueranfly.top

[G08] 静态方法与属性
来源：http://qzq.jinqigfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aog.mhx1999.top

PHP:  public static function f() {}
来源：http://hxo.haohaochexian.top

JS:   static f() {}
来源：http://vea.hcnkem.com

TS:   static f(): void {}
来源：http://sax.jyoumei.cn

Java: static void f() {}
来源：http://dxg.daxiang520.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fbm.hammf.cn

Ruby: def self.f; end
来源：http://mad.jinqigfzy.top

C#:   public static void F() {}
来源：http://mww.wangdashe.top

[G09] 接口 / 抽象类
来源：http://pjh.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://mky.aizwys.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rwr.chenjidiqi.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://poh.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://eve.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://nsx.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://sud.hesvh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dkf.ppjwa.cn

C#:   interface IShape { double Area(); }
来源：http://tas.xylfe.cn

[G10] 访问控制
来源：http://mvk.fzhhl.top

Py:   约定 _protected / __private（不强制）
来源：http://epe.zhixingplan.top

PHP:  public / protected / private
来源：http://qay.hnqzz.top

JS:   #private 字段；其余公开
来源：http://zxr.daria6918.cn

TS:   public / protected / private
来源：http://gjj.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://ewq.wangdashe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zgz.aibaodan.cn

Ruby: public / protected / private
来源：http://kro.hnqzz.top

C#:   public / protected / private / internal
来源：http://mjd.iojbl.cn

[G11] getter / setter
来源：http://ysj.bbcook.cn

Py:   @property 与 @x.setter
来源：http://dmz.pengpengdd.cyou

PHP:  public function getName(): string { return $this->name; }
来源：http://uhd.yueranfly.top

JS:   get name() { return this._name; }
来源：http://inj.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://htn.andypj.xyz

Java: public String getName() { return name; }
来源：http://xzh.hnxiangtu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mng.xuanzx.com

Ruby: attr_accessor :name
来源：http://sgj.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://qyf.yvedp.cn

[G12] 对象转字符串
来源：http://cda.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://tvz.chenlongwang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ogm.hnqzz.top

JS:   toString() { return this.name; }
来源：http://tlc.yuanzhike.top

TS:   toString(): string { return this.name; }
来源：http://wje.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://ars.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://gko.zhengqikj.top

Ruby: def to_s; @name; end
来源：http://hxb.yj20258.top

C#:   public override string ToString() => Name;
来源：http://xhj.jlsjyb.cn

[G13] 判断对象类型
来源：http://fha.zhengqikj.top

Py:   isinstance(u, User)
来源：http://kjx.xziqi.cn

PHP:  $u instanceof User
来源：http://tky.yj202588.top

JS:   u instanceof User
来源：http://xyl.yongpay.top

TS:   u instanceof User
来源：http://msr.zhaomingkeji.xyz

Java: u instanceof User
来源：http://npy.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wze.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://gvy.wangshuangyany.cn

C#:   u is User
来源：http://ysv.birdmap.top

[G14] 数据类 / record
来源：http://ukg.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fnz.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://uhx.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://yyd.andypj.xyz

TS:   type User = { name: string; age: number };
来源：http://dvu.zhengqikj.top

Java: record User(String name, int age) {}
来源：http://rsw.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://njc.yj202588.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ody.yj20258.top

C#:   record User(string Name, int Age);
来源：http://ghp.zdqjudy.top

[G15] 枚举
来源：http://oor.ydjk.org.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jde.jianghu66.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://azm.ivvv.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uth.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mzo.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://yoy.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kyg.jinghuilouyu.cn

Ruby: Color = %i[red green].freeze
来源：http://mae.nanxinkj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dzu.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://lgs.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wab.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://vaz.zycfv.cn

JS:   Object.entries(obj)
来源：http://son.yongpay.top

TS:   Object.entries(obj)
来源：http://qgi.meibo888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oqr.birdmap.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bog.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://cpn.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://amv.hywenlv.cn

================================================================================
来源：http://jtt.wangshuangyany.cn

H. 异常与错误处理
来源：http://pgj.zhixingplan.top

================================================================================
来源：http://uxu.cqqwz.cn

[H01] try / catch 基础
来源：http://acp.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yea.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mlx.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dqk.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://szr.fanxiaobao.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xvy.zhijiandao.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fcx.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bst.hongshengwenyu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tqz.chenzaomai.com

[H02] finally / ensure 收尾
来源：http://get.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://zep.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gky.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pzi.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://tgj.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://qxu.52xcode.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tcd.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://teh.redwolf501.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yyn.yonumen.top

[H03] 主动抛出异常
来源：http://vlj.redwolf501.top

Py:   raise ValueError("错误信息")
来源：http://vef.c1oappe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lhw.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://jvp.yuanzhike.top

TS:   throw new Error("错误信息");
来源：http://yck.nwbrower.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dvu.shuidangran.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lzj.sufxvd.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lkq.sweek.top

C#:   throw new ArgumentException("错误信息");
来源：http://rjy.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://gso.svipenyu.cn

Py:   class MyError(Exception): pass
来源：http://imr.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://zms.jinqigufen.top

JS:   class MyError extends Error {}
来源：http://rnp.0kj1m.cn

TS:   class MyError extends Error {}
来源：http://cqg.nanxinkj.top

Java: class MyException extends RuntimeException {}
来源：http://uwf.snrcjt.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bvi.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://bqz.epnwcf.com

C#:   class MyException : Exception {}
来源：http://eat.316326.xyz

[H05] 捕获特定类型
来源：http://gga.gaohongyu789.top

Py:   except ValueError as e:
来源：http://kmi.tian-w.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mfo.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://qys.zycfv.cn

TS:   if (e instanceof TypeError) {}
来源：http://xnr.shanyushiyangtech.top

Java: catch (IOException | SQLException e) {}
来源：http://sns.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nxj.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://oqy.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ujp.316326.xyz

[H06] 可选值 / 空值安全访问
来源：http://ehk.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://xir.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://efy.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://pfl.xuanzx.com

TS:   obj?.a?.b;  d ?? default
来源：http://myg.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://snz.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://oua.andypj.xyz

Ruby: d&.dig(:a, :b)
来源：http://dvq.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://ygd.andypj.xyz

[H07] 断言
来源：http://kvc.birdmap.top

Py:   assert x > 0, "必须为正"
来源：http://jak.guowangkeji.top

PHP:  assert($x > 0);
来源：http://ytw.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://lhj.zhijiandao.cn

TS:   console.assert(x > 0);
来源：http://svh.shzxlz.cn

Java: assert x > 0 : "必须为正";
来源：http://thb.hnxiangtu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fnm.daria6918.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zjr.hongshengwenyu.top

C#:   Debug.Assert(x > 0);
来源：http://rur.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://rex.shzxlz.cn

Py:   str(e);  traceback.format_exc()
来源：http://jcd.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vhk.shanyushiyangtech.top

JS:   e.message;  e.stack
来源：http://vjl.andypj.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://srb.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rsv.pycfn.com

Go:   err.Error()
来源：http://gme.tianlin.xyz

Ruby: e.message;  e.backtrace
来源：http://ulm.zhiwuduotai.top

C#:   e.Message;  e.StackTrace
来源：http://pdl.shzxlz.cn

[H09] 带错误码的异常
来源：http://vkc.c1oappe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lpz.nanxinkj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mue.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uwj.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mad.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xnw.yuxming.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qkz.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://bzg.redwolf501.top

C#:   // 自定义异常类中加 Code 属性
来源：http://esf.daria6918.cn

[H10] 资源自动释放
来源：http://uye.nanxinkj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://maq.zhengqikj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ice.zycfv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pju.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pkw.hongshengwenyu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lmv.hywenlv.cn

Go:   defer f.Close()
来源：http://xbh.zhijiandao.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xql.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fzi.uphjek.com

================================================================================
来源：http://pqv.cqqwz.cn

I. 正则表达式
来源：http://sdl.zdbjq.cn

================================================================================
来源：http://cge.uphjek.com

[I01] 判断是否匹配
来源：http://psg.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nfm.xuetiantiany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nzy.sxryk.cn

JS:   /\d+/.test(s)
来源：http://dof.guannengcc.top

TS:   /\d+/.test(s)
来源：http://piu.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vqr.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qop.hysaishi.cn

Ruby: s.match?(/\d+/)
来源：http://xbq.hammf.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sty.dianchejie.cn

[I02] 提取所有匹配
来源：http://shq.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://nmw.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jby.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zzk.bjfxy.top

TS:   s.match(/\d+/g)
来源：http://vqm.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aiq.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ndq.chenjidiqi.icu

Ruby: s.scan(/\d+/)
来源：http://qyq.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dxx.zhiwuduotai.top

[I03] 提取捕获分组
来源：http://irz.vqdsnc.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oqq.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wao.52xcode.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jdy.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yyj.jqgfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zgy.feifeiyinyue.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hll.yj20258888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wbj.ydzc1.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aoo.yj20258888.top

[I04] 正则替换
来源：http://pom.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pvi.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yyi.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://cjg.mhx1999.top

TS:   s.replace(/\d+/g, "#")
来源：http://pok.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://vxt.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vbo.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ydw.ydjk.org.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xha.sufxvd.cn

[I05] 按正则拆分
来源：http://fmm.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vjf.dashuyun.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wfy.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://rxr.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://zdb.yfazqb.com

Java: s.split("\\s*,\\s*")
来源：http://piv.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://abt.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://not.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gsu.tian-w.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gkn.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://haf.gzhubu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lvn.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ywy.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://coa.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rko.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nud.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bvq.chenzaomai.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yir.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://uut.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uov.dashuyun.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nui.gogol.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hra.guowangkeji.top

TS:   /error/gim
来源：http://rzi.xziqi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dfl.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hds.yfazqb.com

Ruby: s.scan(/error/i)
来源：http://zai.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cmj.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://ebz.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pxm.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://val.jinghuilouyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wki.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wil.yj20258.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zra.vehdjk.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vin.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qgx.cashguo.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ovp.zycfv.cn

================================================================================
来源：http://lhy.tanke756.top

J. 日期与时间
来源：http://iev.shangyingyoupin.top

================================================================================
来源：http://pme.xuetiantiany.cn

[J01] 获取当前时间
来源：http://ihy.tanke756.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://irv.gaohongyu789.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yyp.snrcjt.cn

JS:   new Date();  Date.now()
来源：http://roz.ybcxt.top

TS:   new Date();  Date.now()
来源：http://nyh.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bwz.yvedp.cn

Go:   time.Now()
来源：http://rpv.chenlongwang.top

Ruby: Time.now
来源：http://thw.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rqc.iojbl.cn

[J02] 格式化输出
来源：http://fot.yuanzhike.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sqd.daxiang520.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gwl.sxryk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hhk.dashuyun.cn

TS:   d.toISOString()
来源：http://lpw.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://amk.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eeq.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pod.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gwj.ydzc1.top

[J03] 字符串解析为日期
来源：http://lez.cheryme.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gug.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ksv.tianlin.xyz

JS:   new Date("2024-01-02")
来源：http://rvv.daxiang520.top

TS:   new Date("2024-01-02")
来源：http://rih.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://kzq.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pzs.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://vtw.zhijiandao.cn


<!-- 参考信息 -->