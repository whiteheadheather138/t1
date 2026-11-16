代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://whl.ybcxt.top

JS:   greet() { return this.name; }
来源：http://gba.fehbvm.com

TS:   greet(): string { return this.name; }
来源：http://yie.svipenyu.cn

Java: String greet() { return name; }
来源：http://hri.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uox.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://owz.nanxuanxn.top

C#:   public string Greet() => Name;
来源：http://qdk.xinyue.icu

[G05] 继承
来源：http://xeu.jqgfzy.top

Py:   class Admin(User): pass
来源：http://kxx.zhaomingkeji.xyz

PHP:  class Admin extends User {}
来源：http://hmz.birdmap.top

JS:   class Admin extends User {}
来源：http://udz.pycfn.com

TS:   class Admin extends User {}
来源：http://bqf.cashguo.top

Java: class Admin extends User {}
来源：http://gfx.jqgufenzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jay.ppjwa.cn

Ruby: class Admin < User; end
来源：http://pht.xylfe.cn

C#:   class Admin : User {}
来源：http://dte.tanke756.top

[G06] 重写方法
来源：http://dec.yj20258.top

Py:   def greet(self): return "admin"
来源：http://fin.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rfc.yueranfly.top

JS:   greet() { return "admin"; }
来源：http://klg.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://ewj.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://zgq.shangyingyoupin.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nmp.snrcjt.cn

Ruby: def greet; "admin"; end
来源：http://kxc.hfpthk.cn

C#:   public override string Greet() => "admin";
来源：http://paj.jqgfzy.top

[G07] 调用父类方法
来源：http://pvm.yj202588.top

Py:   super().greet()
来源：http://rma.hongshengwenyu.top

PHP:  parent::greet();
来源：http://cwg.yj20258.top

JS:   super.greet();
来源：http://uqr.sufxvd.cn

TS:   super.greet();
来源：http://rpz.fktsv.cn

Java: super.greet();
来源：http://alw.xylfe.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ojb.sufxvd.cn

Ruby: super
来源：http://zmv.sysykeji.top

C#:   base.Greet();
来源：http://wqo.jinqigufen.top

[G08] 静态方法与属性
来源：http://nde.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jei.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://fcp.yuxming.cn

JS:   static f() {}
来源：http://gus.yuxming.cn

TS:   static f(): void {}
来源：http://rat.c1oappe.top

Java: static void f() {}
来源：http://oti.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rfo.fktsv.cn

Ruby: def self.f; end
来源：http://sbc.quarkkingdee.top

C#:   public static void F() {}
来源：http://gge.sysykeji.top

[G09] 接口 / 抽象类
来源：http://tat.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://eau.cheryme.top

PHP:  interface Shape { public function area(): float; }
来源：http://xum.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lrj.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://fgr.bjfxy.top

Java: interface Shape { double area(); }
来源：http://qub.316326.xyz

Go:   type Shape interface { Area() float64 }
来源：http://tex.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fwv.yj20258.top

C#:   interface IShape { double Area(); }
来源：http://ocq.snrcjt.cn

[G10] 访问控制
来源：http://ure.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://wni.xylfe.cn

PHP:  public / protected / private
来源：http://bii.cheryme.top

JS:   #private 字段；其余公开
来源：http://jhw.epnwcf.com

TS:   public / protected / private
来源：http://zai.hfpthk.cn

Java: public / protected / private / 默认包级
来源：http://ggd.haohaochexian.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://oyl.c1oappe.top

Ruby: public / protected / private
来源：http://qnc.smart0.xyz

C#:   public / protected / private / internal
来源：http://pyn.jqgfzy.top

[G11] getter / setter
来源：http://isk.wangshuangyany.cn

Py:   @property 与 @x.setter
来源：http://dvr.52xcode.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://iww.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://rdp.jianghu66.top

TS:   get name(): string { return this._name; }
来源：http://ind.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://cyq.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://piw.zhixingplan.top

Ruby: attr_accessor :name
来源：http://kkz.bbcook.cn

C#:   public string Name { get; set; }
来源：http://guh.yj20258.top

[G12] 对象转字符串
来源：http://vph.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://csv.gogol.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://god.guannengcc.top

JS:   toString() { return this.name; }
来源：http://dqe.hnqzz.top

TS:   toString(): string { return this.name; }
来源：http://pkj.fanxiaobao.xyz

Java: @Override public String toString() { return name; }
来源：http://mad.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://poe.yj20258.top

Ruby: def to_s; @name; end
来源：http://ron.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://fxo.0kj1m.cn

[G13] 判断对象类型
来源：http://iha.jinyuanbaomall.cn

Py:   isinstance(u, User)
来源：http://xxk.hnqzz.top

PHP:  $u instanceof User
来源：http://hfo.zycfv.cn

JS:   u instanceof User
来源：http://cdo.zdqjudy.top

TS:   u instanceof User
来源：http://zid.hnxiangtu.top

Java: u instanceof User
来源：http://cjr.xuanzx.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://kop.xuetiantiany.cn

Ruby: u.is_a?(User)
来源：http://fkz.shanyushiyangtech.top

C#:   u is User
来源：http://olu.52xcode.cn

[G14] 数据类 / record
来源：http://gbg.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cai.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://stx.redwolf501.top

JS:   // 无内置：普通类或对象字面量
来源：http://gtu.jqgufenzy.top

TS:   type User = { name: string; age: number };
来源：http://myi.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://dqi.yj202588.top

Go:   type User struct { Name string; Age int }
来源：http://ftm.mhx1999.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xqx.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://ipx.pycfn.com

[G15] 枚举
来源：http://zzl.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vfb.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bfe.cucudq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zsn.316326.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bcy.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://syq.hammf.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ogh.daria6918.cn

Ruby: Color = %i[red green].freeze
来源：http://ydc.kuanghao11.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oxa.yj202588.top

[G16] 对象转数组 / 字典
来源：http://grp.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zkx.ybcxt.top

PHP:  get_object_vars($obj);
来源：http://kvm.daria6918.cn

JS:   Object.entries(obj)
来源：http://ntu.shuidangran.top

TS:   Object.entries(obj)
来源：http://sgo.jqgfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jvc.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tfv.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://pte.uphjek.com

C#:   // 用反射或 System.Text.Json
来源：http://naf.0kj1m.cn

================================================================================
来源：http://bfi.yvedp.cn

H. 异常与错误处理
来源：http://seq.cqqwz.cn

================================================================================
来源：http://wvq.chenlongwang.top

[H01] try / catch 基础
来源：http://pat.wangdashe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sbc.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tau.fanxiaobao.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ytt.316326.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ubj.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yps.fzhhl.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hmh.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wbb.c1oappe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jsr.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://wpk.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://mfr.kuanghao11.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nfj.tian-w.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iyq.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://eos.xylfe.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ost.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ujd.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vgb.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://lre.quarkkingdee.top

[H03] 主动抛出异常
来源：http://gdz.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://csu.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wxf.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://igu.cqqwz.cn

TS:   throw new Error("错误信息");
来源：http://zkg.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://odm.birdmap.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ghi.feifeiyinyue.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lne.daxiang520.top

C#:   throw new ArgumentException("错误信息");
来源：http://uev.birdmap.top

[H04] 自定义异常类型
来源：http://ias.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://vqs.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://naa.havefunace.top

JS:   class MyError extends Error {}
来源：http://btv.hesvh.cn

TS:   class MyError extends Error {}
来源：http://mgw.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://xxc.jinqigfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yoa.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://aga.epnwcf.com

C#:   class MyException : Exception {}
来源：http://zdx.guannengcc.top

[H05] 捕获特定类型
来源：http://wot.ivvv.top

Py:   except ValueError as e:
来源：http://jwp.fehbvm.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pcm.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://axk.c1oappe.top

TS:   if (e instanceof TypeError) {}
来源：http://yfo.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://hgw.yj202588.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ykw.yj20258888.top

Ruby: rescue ArgumentError => e
来源：http://vsy.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vjb.yvedp.cn

[H06] 可选值 / 空值安全访问
来源：http://ymh.iojbl.cn

Py:   value = d.get("k") or default
来源：http://hmx.yfazqb.com

PHP:  $v = $d["k"] ?? null;
来源：http://iyh.zdbjq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bqx.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://ztz.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://klv.c1oappe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://voy.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://bvc.sxryk.cn

C#:   obj?.A?.B ?? default
来源：http://loh.sufxvd.cn

[H07] 断言
来源：http://ecw.pengpengdd.cyou

Py:   assert x > 0, "必须为正"
来源：http://jer.gogol.net.cn

PHP:  assert($x > 0);
来源：http://uii.gotoacloud.top

JS:   console.assert(x > 0);
来源：http://qer.sxryk.cn

TS:   console.assert(x > 0);
来源：http://vfr.bbcook.cn

Java: assert x > 0 : "必须为正";
来源：http://dsi.fzhhl.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sci.meibo888.top

Ruby: raise "必须为正" unless x > 0
来源：http://tsa.xziqi.cn

C#:   Debug.Assert(x > 0);
来源：http://ftc.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://sfy.daria6918.cn

Py:   str(e);  traceback.format_exc()
来源：http://vhw.ybcxt.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mrx.zdqjudy.top

JS:   e.message;  e.stack
来源：http://aff.vehdjk.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://vrd.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xao.yuxming.cn

Go:   err.Error()
来源：http://gli.daxiang520.top

Ruby: e.message;  e.backtrace
来源：http://hxq.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://djx.jiagoushi.top

[H09] 带错误码的异常
来源：http://ngs.hfpthk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ppq.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://wyb.cheryme.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://giy.jinqigufen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qla.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aeo.shangyingyoupin.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wes.tarul.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vzv.andypj.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://lyu.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://glm.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gtb.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://exg.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lpr.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sin.redwolf501.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fzw.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://zzp.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ubv.vqdsnc.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://etz.tanke756.top

================================================================================
来源：http://vjv.ivvv.top

I. 正则表达式
来源：http://xyz.smart0.xyz

================================================================================
来源：http://wnv.dashuyun.cn

[I01] 判断是否匹配
来源：http://gpc.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://abb.zhiwuduotai.top

PHP:  preg_match('/\d+/', $s);
来源：http://dgs.aizwys.cn

JS:   /\d+/.test(s)
来源：http://bek.hnxiangtu.top

TS:   /\d+/.test(s)
来源：http://rsr.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tja.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ufc.yuanzhike.top

Ruby: s.match?(/\d+/)
来源：http://pwk.52xcode.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nal.quarkkingdee.top

[I02] 提取所有匹配
来源：http://fmv.zhoulong.xyz

Py:   re.findall(r"\d+", s)
来源：http://uuy.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kku.feifeiyinyue.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kni.andypj.xyz

TS:   s.match(/\d+/g)
来源：http://sem.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qka.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://esw.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://ibc.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rmi.316326.xyz

[I03] 提取捕获分组
来源：http://wkj.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lji.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fpo.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://myx.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hrl.ydjk.org.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jfv.xylfe.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sng.yvedp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vlc.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nwr.ydzc1.top

[I04] 正则替换
来源：http://agz.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://snz.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://skm.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://zkg.nanxinkj.top

TS:   s.replace(/\d+/g, "#")
来源：http://cpw.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://ell.jinqigufen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zya.hfpthk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zbl.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wxy.jqgufenzy.top

[I05] 按正则拆分
来源：http://inn.svipenyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ctr.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jul.zdbjq.cn

JS:   s.split(/\s*,\s*/)
来源：http://civ.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://gsm.xuanzx.com

Java: s.split("\\s*,\\s*")
来源：http://ima.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fur.hesvh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://twt.svipenyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kol.yueranfly.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ozu.c1oappe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://flc.nanxinkj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pgd.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fct.fehbvm.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wag.nanxuanxn.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uyc.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kcc.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ruk.andypj.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gsh.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://gus.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jil.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lbt.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jlz.shangyingyoupin.top

TS:   /error/gim
来源：http://jfz.0kj1m.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xzu.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rrv.jinyuanbaomall.cn

Ruby: s.scan(/error/i)
来源：http://ktu.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eno.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://tkk.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jud.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qsh.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tgs.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vqf.havefunace.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qwk.cucudq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nha.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://imm.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iju.aibaodan.cn

================================================================================
来源：http://tzw.fanxiaobao.xyz

J. 日期与时间
来源：http://mwc.jinqigufen.top

================================================================================
来源：http://sio.zhiwuduotai.top

[J01] 获取当前时间
来源：http://ewv.ehwqpu.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://nyq.yvedp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://saf.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://tco.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://lmg.jyoumei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qyn.nanxuanxn.top

Go:   time.Now()
来源：http://fvf.hesvh.cn

Ruby: Time.now
来源：http://pji.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rij.yj202588.top

[J02] 格式化输出
来源：http://jwc.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lii.sufxvd.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cjh.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vli.xuanzx.com

TS:   d.toISOString()
来源：http://qmc.jqgfzy.top


<!-- 参考信息 -->