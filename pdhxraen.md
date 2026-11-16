代发 wailian999

Java: class Admin extends User {}
来源：http://dsj.ywan-chungtsiang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ftj.dashuyun.cn

Ruby: class Admin < User; end
来源：http://bqx.aizwys.cn

C#:   class Admin : User {}
来源：http://mzs.nanxuanxn.top

[G06] 重写方法
来源：http://ghf.zhengqikj.top

Py:   def greet(self): return "admin"
来源：http://ihk.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ofi.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://spy.yj20258.top

TS:   greet(): string { return "admin"; }
来源：http://tyy.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://omb.jinqigfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uzp.bjfxy.top

Ruby: def greet; "admin"; end
来源：http://gkn.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://tgg.hfpthk.cn

[G07] 调用父类方法
来源：http://qrj.gogol.net.cn

Py:   super().greet()
来源：http://wdx.nanxuanxn.top

PHP:  parent::greet();
来源：http://pai.meibo888.top

JS:   super.greet();
来源：http://xaa.cdnleiting.top

TS:   super.greet();
来源：http://ixn.smart0.xyz

Java: super.greet();
来源：http://tvb.yvedp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oya.havefunace.top

Ruby: super
来源：http://fzl.birdmap.top

C#:   base.Greet();
来源：http://ctx.yj20258888.top

[G08] 静态方法与属性
来源：http://rmj.andypj.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bea.tianlin.xyz

PHP:  public static function f() {}
来源：http://zwm.zhaomingkeji.xyz

JS:   static f() {}
来源：http://yel.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://rqm.jqgfzy.top

Java: static void f() {}
来源：http://juz.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jvr.hcnkem.com

Ruby: def self.f; end
来源：http://thy.yanxiufei.cn

C#:   public static void F() {}
来源：http://apf.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://ejy.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://cuu.yongpay.top

PHP:  interface Shape { public function area(): float; }
来源：http://qay.yfazqb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://eul.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://xvl.jianghu66.top

Java: interface Shape { double area(); }
来源：http://ugy.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://gsa.zhiwuduotai.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://npc.sufxvd.cn

C#:   interface IShape { double Area(); }
来源：http://faj.52xcode.cn

[G10] 访问控制
来源：http://zzx.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://qvx.hnqzz.top

PHP:  public / protected / private
来源：http://wsu.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://bwe.hysaishi.cn

TS:   public / protected / private
来源：http://fbt.tarul.cn

Java: public / protected / private / 默认包级
来源：http://mus.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gty.xuetiantiany.cn

Ruby: public / protected / private
来源：http://czj.zhengqikj.top

C#:   public / protected / private / internal
来源：http://vuu.hfpthk.cn

[G11] getter / setter
来源：http://dpv.epnwcf.com

Py:   @property 与 @x.setter
来源：http://eoj.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ldz.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://epf.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://crl.nwbrower.top

Java: public String getName() { return name; }
来源：http://uei.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lrv.havefunace.top

Ruby: attr_accessor :name
来源：http://wfu.sxryk.cn

C#:   public string Name { get; set; }
来源：http://fgu.daxiang520.top

[G12] 对象转字符串
来源：http://osx.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://mir.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xgd.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://exy.ywan-chungtsiang.top

TS:   toString(): string { return this.name; }
来源：http://elg.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://afs.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://fsn.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://vcx.chenlongwang.top

C#:   public override string ToString() => Name;
来源：http://npq.bjfxy.top

[G13] 判断对象类型
来源：http://uaw.aibaodan.cn

Py:   isinstance(u, User)
来源：http://bwy.sweek.top

PHP:  $u instanceof User
来源：http://emg.jqgfzy.top

JS:   u instanceof User
来源：http://dif.fengsongda.top

TS:   u instanceof User
来源：http://qng.zhaomingkeji.xyz

Java: u instanceof User
来源：http://ktk.yj20258888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xye.hesvh.cn

Ruby: u.is_a?(User)
来源：http://zar.chenlongwang.top

C#:   u is User
来源：http://tzb.tarul.cn

[G14] 数据类 / record
来源：http://xpe.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wos.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://mcf.chenjidiqi.icu

JS:   // 无内置：普通类或对象字面量
来源：http://pmk.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://oim.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://kmu.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://pwi.xuanzx.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iqb.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://fdl.sxryk.cn

[G15] 枚举
来源：http://ayl.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://grw.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://wls.cdnleiting.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rjj.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://owm.yuanzhike.top

Java: enum Color { RED, GREEN }
来源：http://wvv.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wda.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://wsm.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cko.shanyushiyangtech.top

[G16] 对象转数组 / 字典
来源：http://kso.zycfv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fwg.bbcook.cn

PHP:  get_object_vars($obj);
来源：http://fvi.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://dib.ppjwa.cn

TS:   Object.entries(obj)
来源：http://sqz.zhongyouzk.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://znf.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yon.birdmap.top

Ruby: obj.instance_variables
来源：http://fvn.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://pmi.yfazqb.com

================================================================================
来源：http://noh.c1oappe.top

H. 异常与错误处理
来源：http://vug.wangshuangyany.cn

================================================================================
来源：http://sru.cashguo.top

[H01] try / catch 基础
来源：http://xnb.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tae.9152youxi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rcv.hywenlv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://san.vqdsnc.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ffh.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dtu.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yxd.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nbp.tanke756.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jyw.sweek.top

[H02] finally / ensure 收尾
来源：http://fiy.9152youxi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vdi.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rml.gaohongyu789.top

JS:   try { f(); } finally { cleanup(); }
来源：http://upa.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://tmb.shangyingyoupin.top

Java: try { f(); } finally { cleanup(); }
来源：http://pvm.shanyushiyangtech.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qgq.nanxinkj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lix.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bha.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://vom.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://sjh.guowangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tth.dianchejie.cn

JS:   throw new Error("错误信息");
来源：http://eus.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://nia.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xzg.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qph.pycfn.com

Ruby: raise ArgumentError, "错误信息"
来源：http://jga.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://zfu.fengsongda.top

[H04] 自定义异常类型
来源：http://xzl.ivvv.top

Py:   class MyError(Exception): pass
来源：http://oqt.yj202588.top

PHP:  class MyError extends RuntimeException {}
来源：http://kkn.jiagoushi.top

JS:   class MyError extends Error {}
来源：http://inm.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://vrm.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://ivr.cdnleiting.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lnl.nanxuanxn.top

Ruby: class MyError < StandardError; end
来源：http://btv.mhx1999.top

C#:   class MyException : Exception {}
来源：http://swt.gogol.net.cn

[H05] 捕获特定类型
来源：http://ckj.jianghu66.top

Py:   except ValueError as e:
来源：http://yyd.quarkkingdee.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yvr.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://nrr.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://aiw.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://nuc.nwbrower.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wwe.bjfxy.top

Ruby: rescue ArgumentError => e
来源：http://pgw.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xpu.jinqigfzy.top

[H06] 可选值 / 空值安全访问
来源：http://oxc.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://zni.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fnf.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://sdx.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://zdd.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lhr.xuanzx.com

Go:   if v, ok := m["k"]; ok { }
来源：http://zmd.meibo888.top

Ruby: d&.dig(:a, :b)
来源：http://wud.yj20258888.top

C#:   obj?.A?.B ?? default
来源：http://yyh.wangdashe.top

[H07] 断言
来源：http://iwd.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://vac.havefunace.top

PHP:  assert($x > 0);
来源：http://jak.tarul.cn

JS:   console.assert(x > 0);
来源：http://luq.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://big.nanxinkj.top

Java: assert x > 0 : "必须为正";
来源：http://axq.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://usw.aizwys.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xhx.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://pjf.mhx1999.top

[H08] 获取错误信息与堆栈
来源：http://suu.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://inr.chenzaomai.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://idx.nwbrower.top

JS:   e.message;  e.stack
来源：http://ekt.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mhh.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qig.yj20258.top

Go:   err.Error()
来源：http://fvg.hysaishi.cn

Ruby: e.message;  e.backtrace
来源：http://kzn.vqdsnc.cn

C#:   e.Message;  e.StackTrace
来源：http://qmj.tianlin.xyz

[H09] 带错误码的异常
来源：http://gyi.ctjpmb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hqn.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tir.jinqigufen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xtt.ehwqpu.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jie.ctjpmb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zvv.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cbl.haohaochexian.top

Ruby: raise MyError.new("fail", 500)
来源：http://iiw.guowangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mhh.wangshuangyany.cn

[H10] 资源自动释放
来源：http://lhm.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ajd.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pzr.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hkh.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fqu.ydjk.org.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uwk.gaohongyu789.top

Go:   defer f.Close()
来源：http://uer.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qng.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://quk.hammf.cn

================================================================================
来源：http://nua.yj202588.top

I. 正则表达式
来源：http://mob.zhongyouzk.top

================================================================================
来源：http://oqi.ydjk.org.cn

[I01] 判断是否匹配
来源：http://jxf.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rxo.jianghu66.top

PHP:  preg_match('/\d+/', $s);
来源：http://iro.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://clu.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://bip.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zzx.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tjc.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://xmo.zhongyouzk.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jsl.vehdjk.com

[I02] 提取所有匹配
来源：http://edi.ybcxt.top

Py:   re.findall(r"\d+", s)
来源：http://sfz.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gpk.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://onc.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://byh.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://smd.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ptr.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://hxl.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zng.yanxiufei.cn

[I03] 提取捕获分组
来源：http://hjq.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://huk.sjlbkw.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sbp.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ytr.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hsv.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dzh.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://efy.zycfv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ycx.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fot.ivvv.top

[I04] 正则替换
来源：http://dma.hywenlv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dge.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tpq.hammf.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ivp.zhengqikj.top

TS:   s.replace(/\d+/g, "#")
来源：http://ypc.chenlongwang.top

Java: s.replaceAll("\\d+", "#")
来源：http://wlk.mhx1999.top

Go:   re.ReplaceAllString(s, "#")
来源：http://roc.jyoumei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://blz.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nio.ivvv.top

[I05] 按正则拆分
来源：http://qjn.nanxuanxn.top

Py:   re.split(r"\s*,\s*", s)
来源：http://php.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qks.aizwys.cn

JS:   s.split(/\s*,\s*/)
来源：http://cmg.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://ggf.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://opu.xziqi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uye.yueranfly.top

Ruby: s.split(/\s*,\s*/)
来源：http://mbe.jinyuanbaomall.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eiu.guowangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xkd.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jgj.epnwcf.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zdw.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lkr.yj20258888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tic.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lxs.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oib.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nvg.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dep.tian-w.cn

[I07] 忽略大小写与多行模式
来源：http://mnl.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nud.fanxiaobao.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nne.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lla.nanxuanxn.top

TS:   /error/gim
来源：http://uxz.ydzc1.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wtd.hammf.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gwi.pycfn.com

Ruby: s.scan(/error/i)
来源：http://ucq.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pqv.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://huz.cashguo.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sse.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ekc.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qcz.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://okc.jinqigfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://faf.ywan-chungtsiang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nrd.hcnkem.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dop.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ywr.jiagoushi.top

================================================================================
来源：http://hcq.quarkkingdee.top

J. 日期与时间
来源：http://qgd.shanyushiyangkeji.top

================================================================================
来源：http://ptb.fehbvm.com

[J01] 获取当前时间
来源：http://txr.tarul.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ivq.9152youxi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eyw.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://lnn.sxryk.cn

TS:   new Date();  Date.now()
来源：http://zqx.yvedp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bgc.ehwqpu.com

Go:   time.Now()
来源：http://smq.hfpthk.cn

Ruby: Time.now
来源：http://aeo.jiagoushi.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://riu.gotoacloud.top

[J02] 格式化输出
来源：http://ogb.daxiang520.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hup.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jkn.quarkkingdee.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jez.quarkkingdee.top

TS:   d.toISOString()
来源：http://avr.jinyuanbaomall.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dgv.sufxvd.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ytf.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sjn.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jyc.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://rry.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hxg.mhx1999.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://org.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://wkh.jqgfzy.top

TS:   new Date("2024-01-02")
来源：http://qzp.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://ixm.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://htw.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://qev.hcnkem.com


<!-- 参考信息 -->