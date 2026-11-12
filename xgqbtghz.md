代发 wailian999

Ruby: @name = "x"
来源：http://fgo.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ycu.redwolf501.top

[G04] 定义方法
来源：http://cgh.ehwqpu.com

Py:   def greet(self): return self.name
来源：http://bxx.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sev.ehwqpu.com

JS:   greet() { return this.name; }
来源：http://lbo.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://xym.tarul.cn

Java: String greet() { return name; }
来源：http://gig.dashuyun.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://izb.dashuyun.cn

Ruby: def greet; @name; end
来源：http://wwj.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://gfk.zhoulong.xyz

[G05] 继承
来源：http://qfh.hywenlv.cn

Py:   class Admin(User): pass
来源：http://exq.fktsv.cn

PHP:  class Admin extends User {}
来源：http://taz.redwolf501.top

JS:   class Admin extends User {}
来源：http://ybo.cucudq.cn

TS:   class Admin extends User {}
来源：http://iwe.jqgfzy.top

Java: class Admin extends User {}
来源：http://wrb.fehbvm.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kjk.epnwcf.com

Ruby: class Admin < User; end
来源：http://cuj.zdqjudy.top

C#:   class Admin : User {}
来源：http://mxn.guannengcc.top

[G06] 重写方法
来源：http://wsy.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://xxj.jinqigfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://phc.yangfankeji.com

JS:   greet() { return "admin"; }
来源：http://suh.sufxvd.cn

TS:   greet(): string { return "admin"; }
来源：http://fsm.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://osy.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ukm.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://ffy.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://ovb.9152youxi.cn

[G07] 调用父类方法
来源：http://adw.jqgufenzy.top

Py:   super().greet()
来源：http://knx.gzhubu.top

PHP:  parent::greet();
来源：http://rgk.yvedp.cn

JS:   super.greet();
来源：http://esr.xinyue.icu

TS:   super.greet();
来源：http://yzl.316326.xyz

Java: super.greet();
来源：http://fmn.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fvj.aizwys.cn

Ruby: super
来源：http://syz.sufxvd.cn

C#:   base.Greet();
来源：http://oxr.cucudq.cn

[G08] 静态方法与属性
来源：http://kio.guowangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bor.hesvh.cn

PHP:  public static function f() {}
来源：http://wio.snrcjt.cn

JS:   static f() {}
来源：http://atg.jianghu66.top

TS:   static f(): void {}
来源：http://taf.zdbjq.cn

Java: static void f() {}
来源：http://vku.chenlongwang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://spv.iojbl.cn

Ruby: def self.f; end
来源：http://ihv.guannengcc.top

C#:   public static void F() {}
来源：http://eae.jianghu66.top

[G09] 接口 / 抽象类
来源：http://uys.hfpthk.cn

Py:   from abc import ABC, abstractmethod
来源：http://dzo.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jnh.shuidangran.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bxd.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://det.yanxiufei.cn

Java: interface Shape { double area(); }
来源：http://owp.hnqzz.top

Go:   type Shape interface { Area() float64 }
来源：http://pdn.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ght.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://ond.fanxiaobao.xyz

[G10] 访问控制
来源：http://mjh.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://gxu.9152youxi.cn

PHP:  public / protected / private
来源：http://rdf.fanxiaobao.xyz

JS:   #private 字段；其余公开
来源：http://juk.wangshuangyany.cn

TS:   public / protected / private
来源：http://ccf.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://gej.ppjwa.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://iyu.sufxvd.cn

Ruby: public / protected / private
来源：http://kbh.birdmap.top

C#:   public / protected / private / internal
来源：http://fzq.andypj.xyz

[G11] getter / setter
来源：http://gkv.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://nvq.0kj1m.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vcy.yueranfly.top

JS:   get name() { return this._name; }
来源：http://odq.52xcode.cn

TS:   get name(): string { return this._name; }
来源：http://rlk.jqgfzy.top

Java: public String getName() { return name; }
来源：http://vyv.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sbs.ybcxt.top

Ruby: attr_accessor :name
来源：http://ltp.hammf.cn

C#:   public string Name { get; set; }
来源：http://ofg.zhoulong.xyz

[G12] 对象转字符串
来源：http://btn.hnqzz.top

Py:   def __str__(self): return self.name
来源：http://cdl.smart0.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://sws.jqgufenzy.top

JS:   toString() { return this.name; }
来源：http://rmd.meibo888.top

TS:   toString(): string { return this.name; }
来源：http://qar.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://ufg.xuetiantiany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://her.bjfxy.top

Ruby: def to_s; @name; end
来源：http://sks.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://zib.xziqi.cn

[G13] 判断对象类型
来源：http://fmi.ivvv.top

Py:   isinstance(u, User)
来源：http://mos.gzhubu.top

PHP:  $u instanceof User
来源：http://zqk.wangdashe.top

JS:   u instanceof User
来源：http://ykq.yj202588.top

TS:   u instanceof User
来源：http://xpd.sufxvd.cn

Java: u instanceof User
来源：http://rrd.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://rml.pengpengdd.cyou

Ruby: u.is_a?(User)
来源：http://ezv.uphjek.com

C#:   u is User
来源：http://dpb.dashuyun.cn

[G14] 数据类 / record
来源：http://jae.ywan-chungtsiang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uzd.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://wiu.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://dhd.fktsv.cn

TS:   type User = { name: string; age: number };
来源：http://ssh.cheryme.top

Java: record User(String name, int age) {}
来源：http://cfb.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://uck.yj202588.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lye.snrcjt.cn

C#:   record User(string Name, int Age);
来源：http://qew.yangfankeji.com

[G15] 枚举
来源：http://rqv.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vrd.zhoulong.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://shu.yonumen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ihu.havefunace.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jnw.yanxiufei.cn

Java: enum Color { RED, GREEN }
来源：http://gar.tian-w.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mvg.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://moj.bbcook.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kci.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://ydk.meibo888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pba.zhaomingkeji.xyz

PHP:  get_object_vars($obj);
来源：http://tbp.cheryme.top

JS:   Object.entries(obj)
来源：http://wfu.9152youxi.cn

TS:   Object.entries(obj)
来源：http://qpa.gogol.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fvq.zhijiandao.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qww.smart0.xyz

Ruby: obj.instance_variables
来源：http://jgb.cheryme.top

C#:   // 用反射或 System.Text.Json
来源：http://lub.yj202588.top

================================================================================
来源：http://rcu.jinghuilouyu.cn

H. 异常与错误处理
来源：http://dqb.ppjwa.cn

================================================================================
来源：http://fwg.jyoumei.cn

[H01] try / catch 基础
来源：http://nmu.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ehj.ywan-chungtsiang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://inu.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wgz.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mnu.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://evs.redwolf501.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://urm.cqqwz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ryy.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xja.ehwqpu.com

[H02] finally / ensure 收尾
来源：http://kjs.ywan-chungtsiang.top

Py:   try: f()⏎finally: cleanup()
来源：http://usy.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fny.meibo888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://elu.shanyushiyangtech.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mkg.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://yaa.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://szk.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vlo.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://jeq.mhx1999.top

[H03] 主动抛出异常
来源：http://tes.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://jdj.jiagoushi.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zvj.uphjek.com

JS:   throw new Error("错误信息");
来源：http://acc.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://ngk.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qrt.zhixingplan.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wmf.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wlj.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://eek.fzhhl.top

[H04] 自定义异常类型
来源：http://svq.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://lza.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://ejc.quarkkingdee.top

JS:   class MyError extends Error {}
来源：http://wtv.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://qlu.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://wqv.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sfm.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://lyu.fengsongda.top

C#:   class MyException : Exception {}
来源：http://izt.sxryk.cn

[H05] 捕获特定类型
来源：http://znr.zhengqikj.top

Py:   except ValueError as e:
来源：http://ggp.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zrg.zhongyouzk.top

JS:   if (e instanceof TypeError) {}
来源：http://fel.yj20258.top

TS:   if (e instanceof TypeError) {}
来源：http://mqe.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://rly.pengpengdd.cyou

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fnm.ydzc1.top

Ruby: rescue ArgumentError => e
来源：http://wym.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ntm.bbcook.cn

[H06] 可选值 / 空值安全访问
来源：http://nlq.fktsv.cn

Py:   value = d.get("k") or default
来源：http://fdj.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mvu.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qax.shuidangran.top

TS:   obj?.a?.b;  d ?? default
来源：http://lnf.jiagoushi.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ilb.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tia.yuanzhike.top

Ruby: d&.dig(:a, :b)
来源：http://dao.daria6918.cn

C#:   obj?.A?.B ?? default
来源：http://tqr.chenzaomai.com

[H07] 断言
来源：http://koi.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://iog.cdnleiting.top

PHP:  assert($x > 0);
来源：http://vvr.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://ueh.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://sjc.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://bua.ywan-chungtsiang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ase.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://owi.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://nzv.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://pej.zycfv.cn

Py:   str(e);  traceback.format_exc()
来源：http://mkc.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cue.shanyushiyangkeji.top

JS:   e.message;  e.stack
来源：http://mgi.jianghu66.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gqo.zhijiandao.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pwf.ydjk.org.cn

Go:   err.Error()
来源：http://ibh.vehdjk.com

Ruby: e.message;  e.backtrace
来源：http://msx.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://lhm.yanxiufei.cn

[H09] 带错误码的异常
来源：http://ddt.quarkkingdee.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pqd.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jho.fanxiaobao.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rwf.shangyingyoupin.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kod.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sob.nanxuanxn.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gyg.yangfankeji.com

Ruby: raise MyError.new("fail", 500)
来源：http://qfr.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gru.ybcxt.top

[H10] 资源自动释放
来源：http://oax.jqgufenzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://sck.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qcj.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://awz.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gcz.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ynj.fktsv.cn

Go:   defer f.Close()
来源：http://jgq.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xun.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nsv.52xcode.cn

================================================================================
来源：http://qjk.meibo888.top

I. 正则表达式
来源：http://pdc.bjfxy.top

================================================================================
来源：http://sgr.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://roz.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gex.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tqd.guannengcc.top

JS:   /\d+/.test(s)
来源：http://xwn.aibaodan.cn

TS:   /\d+/.test(s)
来源：http://zlf.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dyz.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ybb.ybcxt.top

Ruby: s.match?(/\d+/)
来源：http://qxx.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iah.ydzc1.top

[I02] 提取所有匹配
来源：http://vio.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://vlb.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zzr.zhongyouzk.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rwo.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://fdt.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sbq.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://imy.wangshuangyany.cn

Ruby: s.scan(/\d+/)
来源：http://zin.yueranfly.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kfn.zhixingplan.top

[I03] 提取捕获分组
来源：http://est.jinqigufen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://olx.vehdjk.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cas.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jvc.guannengcc.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://plh.yongpay.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qdo.gogol.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zso.feifeiyinyue.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cti.quarkkingdee.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jmr.hfpthk.cn

[I04] 正则替换
来源：http://lzg.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://oad.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vke.chenzaomai.com

JS:   s.replace(/\d+/g, "#")
来源：http://zvb.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://auo.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://pos.kuanghao11.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pik.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://obk.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hnb.haohaochexian.top

[I05] 按正则拆分
来源：http://mwb.fengsongda.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ksp.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://syh.hfpthk.cn

JS:   s.split(/\s*,\s*/)
来源：http://kiq.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://xum.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://qfi.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eoq.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://qsp.wangdashe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oly.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mwn.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qdb.zdqjudy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yre.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mlu.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ykh.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fsd.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pqq.yfazqb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kcx.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ldw.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://sui.jinqigufen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pix.sweek.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tlf.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://amu.hywenlv.cn

TS:   /error/gim
来源：http://niy.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kdy.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uie.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://jbv.yvedp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xgl.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://cis.jinqigufen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hwx.hnxiangtu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ove.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lhh.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://prk.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://goc.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ukn.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rat.yuanzhike.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jdi.aizwys.cn

================================================================================
来源：http://ell.tanke756.top

J. 日期与时间
来源：http://ukg.jinyuanbaomall.cn

================================================================================
来源：http://fau.gogol.net.cn

[J01] 获取当前时间
来源：http://rik.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://zma.ehwqpu.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lnf.hammf.cn

JS:   new Date();  Date.now()
来源：http://oty.bbcook.cn

TS:   new Date();  Date.now()
来源：http://ptv.sjlbkw.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ekz.guannengcc.top

Go:   time.Now()
来源：http://mds.0kj1m.cn

Ruby: Time.now
来源：http://nst.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ggp.shanyushiyangkeji.top

[J02] 格式化输出
来源：http://bfl.bjfxy.top


<!-- 参考信息 -->