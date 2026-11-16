代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://jhq.tanke756.top

Ruby: def greet; @name; end
来源：http://lur.daxiang520.top

C#:   public string Greet() => Name;
来源：http://gtj.chenlongwang.top

[G05] 继承
来源：http://rjw.dianchejie.cn

Py:   class Admin(User): pass
来源：http://ivu.quarkkingdee.top

PHP:  class Admin extends User {}
来源：http://hyo.hnqzz.top

JS:   class Admin extends User {}
来源：http://dbt.chenjidiqi.icu

TS:   class Admin extends User {}
来源：http://smb.xylfe.cn

Java: class Admin extends User {}
来源：http://byx.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://umw.chenlongwang.top

Ruby: class Admin < User; end
来源：http://xlv.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://exa.shangyingyoupin.top

[G06] 重写方法
来源：http://kse.sysykeji.top

Py:   def greet(self): return "admin"
来源：http://ozp.gaohongyu789.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xeg.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://xyo.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://gmu.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://ilw.xinyue.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xjv.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://vvd.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://xuk.nanxuanxn.top

[G07] 调用父类方法
来源：http://bwt.hywenlv.cn

Py:   super().greet()
来源：http://qxx.yj20258888.top

PHP:  parent::greet();
来源：http://ton.316326.xyz

JS:   super.greet();
来源：http://dsc.gogol.net.cn

TS:   super.greet();
来源：http://asw.cucudq.cn

Java: super.greet();
来源：http://jhq.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bgx.jianghu66.top

Ruby: super
来源：http://etw.dashuyun.cn

C#:   base.Greet();
来源：http://jpg.hesvh.cn

[G08] 静态方法与属性
来源：http://ofo.wangdashe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wav.jianghu66.top

PHP:  public static function f() {}
来源：http://edy.zdqjudy.top

JS:   static f() {}
来源：http://aml.gogol.net.cn

TS:   static f(): void {}
来源：http://eaf.52xcode.cn

Java: static void f() {}
来源：http://kmk.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wka.hfpthk.cn

Ruby: def self.f; end
来源：http://yam.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://fbn.cashguo.top

[G09] 接口 / 抽象类
来源：http://jny.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://gif.xinyue.icu

PHP:  interface Shape { public function area(): float; }
来源：http://qnt.hcnkem.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://yvg.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://iwt.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://jem.fengsongda.top

Go:   type Shape interface { Area() float64 }
来源：http://gfb.aibaodan.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xml.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://nnq.zhaomingkeji.xyz

[G10] 访问控制
来源：http://xbu.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://sgr.dianchejie.cn

PHP:  public / protected / private
来源：http://sje.gaohongyu789.top

JS:   #private 字段；其余公开
来源：http://enl.shzxlz.cn

TS:   public / protected / private
来源：http://prm.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://emr.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qky.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://frk.fengsongda.top

C#:   public / protected / private / internal
来源：http://czq.wangdashe.top

[G11] getter / setter
来源：http://dtd.hcnkem.com

Py:   @property 与 @x.setter
来源：http://qem.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://rne.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://nnd.yueranfly.top

TS:   get name(): string { return this._name; }
来源：http://vnr.yuanzhike.top

Java: public String getName() { return name; }
来源：http://xcv.epnwcf.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ojs.xylfe.cn

Ruby: attr_accessor :name
来源：http://pgk.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://mcw.hcnkem.com

[G12] 对象转字符串
来源：http://zkg.daria6918.cn

Py:   def __str__(self): return self.name
来源：http://use.sysykeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jok.fengsongda.top

JS:   toString() { return this.name; }
来源：http://rbw.zhongyouzk.top

TS:   toString(): string { return this.name; }
来源：http://zda.bjfxy.top

Java: @Override public String toString() { return name; }
来源：http://nkv.gaohongyu789.top

Go:   func (u User) String() string { return u.Name }
来源：http://btg.shanyushiyangtech.top

Ruby: def to_s; @name; end
来源：http://ffe.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://mcl.zhijiandao.cn

[G13] 判断对象类型
来源：http://tmj.uphjek.com

Py:   isinstance(u, User)
来源：http://pav.hfpthk.cn

PHP:  $u instanceof User
来源：http://bkj.zdbjq.cn

JS:   u instanceof User
来源：http://ajh.ivvv.top

TS:   u instanceof User
来源：http://lwr.andypj.xyz

Java: u instanceof User
来源：http://otr.tian-w.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xfo.hammf.cn

Ruby: u.is_a?(User)
来源：http://xap.wangshuangyany.cn

C#:   u is User
来源：http://upc.aizwys.cn

[G14] 数据类 / record
来源：http://gjg.fzhhl.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gyp.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://hux.quarkkingdee.top

JS:   // 无内置：普通类或对象字面量
来源：http://uei.nanxuanxn.top

TS:   type User = { name: string; age: number };
来源：http://bcv.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://pdr.yuxming.cn

Go:   type User struct { Name string; Age int }
来源：http://ync.jqgfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mfw.ctjpmb.com

C#:   record User(string Name, int Age);
来源：http://aie.aizwys.cn

[G15] 枚举
来源：http://qmr.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://foj.iojbl.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ayk.iojbl.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aum.wangshuangyany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ask.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://etn.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sbz.birdmap.top

Ruby: Color = %i[red green].freeze
来源：http://cfe.jyoumei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oqw.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://kkk.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yyl.nanxinkj.top

PHP:  get_object_vars($obj);
来源：http://src.bjfxy.top

JS:   Object.entries(obj)
来源：http://spd.daxiang520.top

TS:   Object.entries(obj)
来源：http://oqt.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://omm.svipenyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://smn.birdmap.top

Ruby: obj.instance_variables
来源：http://fdo.uphjek.com

C#:   // 用反射或 System.Text.Json
来源：http://mew.tarul.cn

================================================================================
来源：http://gfe.hammf.cn

H. 异常与错误处理
来源：http://cqf.yj20258.top

================================================================================
来源：http://nla.mhx1999.top

[H01] try / catch 基础
来源：http://udp.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rtv.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://reh.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fpj.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zta.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rog.meibo888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rdz.ywan-chungtsiang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xzv.chenzaomai.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yds.tarul.cn

[H02] finally / ensure 收尾
来源：http://czq.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://epx.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nol.fanxiaobao.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://lmx.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://gms.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://bvc.guowangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://txk.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lom.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dof.9152youxi.cn

[H03] 主动抛出异常
来源：http://jhx.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://uzs.jinqigufen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://edp.316326.xyz

JS:   throw new Error("错误信息");
来源：http://wca.feifeiyinyue.top

TS:   throw new Error("错误信息");
来源：http://hym.yueranfly.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vfr.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://olc.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nxn.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ceb.cdnleiting.top

[H04] 自定义异常类型
来源：http://fob.gaohongyu789.top

Py:   class MyError(Exception): pass
来源：http://lyz.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://iuh.vehdjk.com

JS:   class MyError extends Error {}
来源：http://ojs.yfazqb.com

TS:   class MyError extends Error {}
来源：http://vil.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://oar.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rvm.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://ezg.hywenlv.cn

C#:   class MyException : Exception {}
来源：http://isd.yj20258888.top

[H05] 捕获特定类型
来源：http://ics.yvedp.cn

Py:   except ValueError as e:
来源：http://elo.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://itg.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://mbw.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://hkb.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://fmt.sysykeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wvj.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://oym.shzxlz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://trr.zhixingplan.top

[H06] 可选值 / 空值安全访问
来源：http://ezq.ybcxt.top

Py:   value = d.get("k") or default
来源：http://qkh.zhoulong.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://fjz.havefunace.top

JS:   obj?.a?.b;  d ?? default
来源：http://hvv.yj20258888.top

TS:   obj?.a?.b;  d ?? default
来源：http://gar.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://chn.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://shw.zhaomingkeji.xyz

Ruby: d&.dig(:a, :b)
来源：http://uoh.jlsjyb.cn

C#:   obj?.A?.B ?? default
来源：http://zki.svipenyu.cn

[H07] 断言
来源：http://srp.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://egt.52xcode.cn

PHP:  assert($x > 0);
来源：http://pyw.0kj1m.cn

JS:   console.assert(x > 0);
来源：http://duf.zhiwuduotai.top

TS:   console.assert(x > 0);
来源：http://ftv.wangdashe.top

Java: assert x > 0 : "必须为正";
来源：http://lai.fzhhl.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gsg.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://oqh.sweek.top

C#:   Debug.Assert(x > 0);
来源：http://ouk.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://jgs.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://lbj.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mwy.daria6918.cn

JS:   e.message;  e.stack
来源：http://zio.sjlbkw.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fwk.9152youxi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wgg.vehdjk.com

Go:   err.Error()
来源：http://dfh.guowangkeji.top

Ruby: e.message;  e.backtrace
来源：http://huk.zycfv.cn

C#:   e.Message;  e.StackTrace
来源：http://obn.yueranfly.top

[H09] 带错误码的异常
来源：http://olu.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://efg.yj202588.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cel.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qyu.zdqjudy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zbm.jqgufenzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xhp.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fcz.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jxp.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pcx.yangfankeji.com

[H10] 资源自动释放
来源：http://fxz.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rrq.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tff.aizwys.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dom.tian-w.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kup.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jzv.aibaodan.cn

Go:   defer f.Close()
来源：http://qxr.tianlin.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hob.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dfx.aizwys.cn

================================================================================
来源：http://fag.jlsjyb.cn

I. 正则表达式
来源：http://cek.jqgfzy.top

================================================================================
来源：http://xom.zhaomingkeji.xyz

[I01] 判断是否匹配
来源：http://kms.yongpay.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lqt.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sai.daria6918.cn

JS:   /\d+/.test(s)
来源：http://dtc.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://twp.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tkr.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cyv.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://ord.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pna.guowangkeji.top

[I02] 提取所有匹配
来源：http://jbo.hesvh.cn

Py:   re.findall(r"\d+", s)
来源：http://gyi.pengpengdd.cyou

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dwd.ctjpmb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jto.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://ief.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rsz.ydzc1.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://huk.svipenyu.cn

Ruby: s.scan(/\d+/)
来源：http://mox.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nzf.iojbl.cn

[I03] 提取捕获分组
来源：http://byw.wangdashe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://msm.gogol.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pgg.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tou.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cqj.hongshengwenyu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jat.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hee.cashguo.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ccu.andypj.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://djm.hesvh.cn

[I04] 正则替换
来源：http://byq.aizwys.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mtn.fanxiaobao.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qby.chenzaomai.com

JS:   s.replace(/\d+/g, "#")
来源：http://ckc.xuetiantiany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ybr.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://yzy.nanxuanxn.top

Go:   re.ReplaceAllString(s, "#")
来源：http://guy.jinghuilouyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://axi.chenlongwang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zwa.bjfxy.top

[I05] 按正则拆分
来源：http://ecc.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://sbk.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://epd.zhongyouzk.top

JS:   s.split(/\s*,\s*/)
来源：http://ezx.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://sho.zhiwuduotai.top

Java: s.split("\\s*,\\s*")
来源：http://zsk.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mio.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://fha.jqgufenzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eqa.jqgufenzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xav.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wqs.nwbrower.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://glt.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bqx.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mxl.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mqg.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hux.gotoacloud.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fuf.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nfa.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://jwx.sjlbkw.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ntm.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dbj.haohaochexian.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uki.vqdsnc.cn

TS:   /error/gim
来源：http://gsw.cashguo.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fsk.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yda.hnqzz.top

Ruby: s.scan(/error/i)
来源：http://ljw.yfazqb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bit.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://rlw.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://isk.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iez.fehbvm.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jwu.daria6918.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ueo.yj20258888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xie.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://age.smart0.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dut.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qtp.ywan-chungtsiang.top

================================================================================
来源：http://lqf.yfazqb.com

J. 日期与时间
来源：http://hjv.yanxiufei.cn

================================================================================
来源：http://ofq.quarkkingdee.top

[J01] 获取当前时间
来源：http://ptu.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://xha.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://joc.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://lbm.xylfe.cn

TS:   new Date();  Date.now()
来源：http://wte.ctjpmb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://xej.gaohongyu789.top

Go:   time.Now()
来源：http://zmt.sxryk.cn

Ruby: Time.now
来源：http://fzt.tanke756.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://six.snrcjt.cn

[J02] 格式化输出
来源：http://uqb.nwbrower.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zwp.bbcook.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eoe.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cun.ivvv.top

TS:   d.toISOString()
来源：http://hqe.jinqigufen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kzr.quarkkingdee.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cqk.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vmn.yueranfly.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pql.jinqigfzy.top


<!-- 参考信息 -->