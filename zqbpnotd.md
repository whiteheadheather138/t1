代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://bga.cheryme.top

[G07] 调用父类方法
来源：http://fuc.yj202588.top

Py:   super().greet()
来源：http://djz.tianlin.xyz

PHP:  parent::greet();
来源：http://dmg.ivvv.top

JS:   super.greet();
来源：http://xrf.cashguo.top

TS:   super.greet();
来源：http://ssn.hammf.cn

Java: super.greet();
来源：http://ohs.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kdn.yanxiufei.cn

Ruby: super
来源：http://wre.fktsv.cn

C#:   base.Greet();
来源：http://yiv.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://gok.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://psj.xuanzx.com

PHP:  public static function f() {}
来源：http://ric.yuanzhike.top

JS:   static f() {}
来源：http://dcm.aibaodan.cn

TS:   static f(): void {}
来源：http://aqe.yuxming.cn

Java: static void f() {}
来源：http://mnn.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://wkm.hnqzz.top

Ruby: def self.f; end
来源：http://ehk.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://bue.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://oox.hfpthk.cn

Py:   from abc import ABC, abstractmethod
来源：http://xyn.ybcxt.top

PHP:  interface Shape { public function area(): float; }
来源：http://uic.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bzp.sjlbkw.cn

TS:   interface Shape { area(): number; }
来源：http://ltk.yanxiufei.cn

Java: interface Shape { double area(); }
来源：http://dzv.hesvh.cn

Go:   type Shape interface { Area() float64 }
来源：http://zpg.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zed.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://khb.xziqi.cn

[G10] 访问控制
来源：http://szt.sxryk.cn

Py:   约定 _protected / __private（不强制）
来源：http://ber.jqgufenzy.top

PHP:  public / protected / private
来源：http://cgn.fanxiaobao.xyz

JS:   #private 字段；其余公开
来源：http://ddo.nanxuanxn.top

TS:   public / protected / private
来源：http://hsh.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://tfa.nanxuanxn.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zlc.ehwqpu.com

Ruby: public / protected / private
来源：http://bkb.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://mnd.uphjek.com

[G11] getter / setter
来源：http://jpt.cucudq.cn

Py:   @property 与 @x.setter
来源：http://kle.pengpengdd.cyou

PHP:  public function getName(): string { return $this->name; }
来源：http://irc.tianlin.xyz

JS:   get name() { return this._name; }
来源：http://zgd.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://iwy.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://bdl.hammf.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hck.uphjek.com

Ruby: attr_accessor :name
来源：http://nce.feifeiyinyue.top

C#:   public string Name { get; set; }
来源：http://vtb.vehdjk.com

[G12] 对象转字符串
来源：http://tpk.zhijiandao.cn

Py:   def __str__(self): return self.name
来源：http://zqc.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://enb.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://hmp.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://msw.jlsjyb.cn

Java: @Override public String toString() { return name; }
来源：http://xnq.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hhq.zhijiandao.cn

Ruby: def to_s; @name; end
来源：http://zgt.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://onj.hnqzz.top

[G13] 判断对象类型
来源：http://lik.snrcjt.cn

Py:   isinstance(u, User)
来源：http://exf.shzxlz.cn

PHP:  $u instanceof User
来源：http://eqw.aizwys.cn

JS:   u instanceof User
来源：http://sdk.ydjk.org.cn

TS:   u instanceof User
来源：http://hew.gaohongyu789.top

Java: u instanceof User
来源：http://sfv.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qdj.cashguo.top

Ruby: u.is_a?(User)
来源：http://ejm.52xcode.cn

C#:   u is User
来源：http://hyn.jinqigfzy.top

[G14] 数据类 / record
来源：http://gst.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uue.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://ady.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vck.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://fwl.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://rpj.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://vwh.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://idq.316326.xyz

C#:   record User(string Name, int Age);
来源：http://phx.52xcode.cn

[G15] 枚举
来源：http://rwg.ydzc1.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://toq.ydjk.org.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sap.zdbjq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qdx.yueranfly.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eyx.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://kgh.haohaochexian.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://owe.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://pfo.ybcxt.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xlm.shanyushiyangtech.top

[G16] 对象转数组 / 字典
来源：http://urz.ppjwa.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jdu.sjlbkw.cn

PHP:  get_object_vars($obj);
来源：http://wgk.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://tjz.tianlin.xyz

TS:   Object.entries(obj)
来源：http://hzd.shanyushiyangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://weh.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tba.vehdjk.com

Ruby: obj.instance_variables
来源：http://itw.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://orc.bbcook.cn

================================================================================
来源：http://tty.hywenlv.cn

H. 异常与错误处理
来源：http://qjr.ydzc1.top

================================================================================
来源：http://nrh.fengsongda.top

[H01] try / catch 基础
来源：http://hmz.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bws.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wpp.jianghu66.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hgw.jinyuanbaomall.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lcd.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ndz.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sfu.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uus.jyoumei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ngk.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://rnp.cucudq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lpf.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ypo.jqgufenzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zny.sweek.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nhf.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://ndp.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://syl.52xcode.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://twg.sjlbkw.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mua.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://urt.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://hbg.cdnleiting.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xtz.hywenlv.cn

JS:   throw new Error("错误信息");
来源：http://pvt.xuetiantiany.cn

TS:   throw new Error("错误信息");
来源：http://otd.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hxq.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lbj.zhijiandao.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ndk.tarul.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kdk.meibo888.top

[H04] 自定义异常类型
来源：http://ksi.cashguo.top

Py:   class MyError(Exception): pass
来源：http://rir.cqqwz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kjm.tarul.cn

JS:   class MyError extends Error {}
来源：http://jmh.aibaodan.cn

TS:   class MyError extends Error {}
来源：http://skv.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://zqg.sysykeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wqn.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://mwz.yuxming.cn

C#:   class MyException : Exception {}
来源：http://gah.yfazqb.com

[H05] 捕获特定类型
来源：http://iro.quarkkingdee.top

Py:   except ValueError as e:
来源：http://glu.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mei.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://rla.sysykeji.top

TS:   if (e instanceof TypeError) {}
来源：http://jor.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://uml.redwolf501.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ava.sjlbkw.cn

Ruby: rescue ArgumentError => e
来源：http://aip.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://usn.yongpay.top

[H06] 可选值 / 空值安全访问
来源：http://bzq.yfazqb.com

Py:   value = d.get("k") or default
来源：http://cdf.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://tyz.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://fsa.xziqi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jvf.birdmap.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cfs.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://myi.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://osv.zhixingplan.top

C#:   obj?.A?.B ?? default
来源：http://kde.uphjek.com

[H07] 断言
来源：http://cgw.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://gnn.fengsongda.top

PHP:  assert($x > 0);
来源：http://ihs.bbcook.cn

JS:   console.assert(x > 0);
来源：http://hke.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://yrm.chenzaomai.com

Java: assert x > 0 : "必须为正";
来源：http://lkm.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sfd.snrcjt.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pla.sjlbkw.cn

C#:   Debug.Assert(x > 0);
来源：http://pmt.zhongyouzk.top

[H08] 获取错误信息与堆栈
来源：http://lcz.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://jtl.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zrz.tanke756.top

JS:   e.message;  e.stack
来源：http://nca.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://plo.zhiwuduotai.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cfv.mhx1999.top

Go:   err.Error()
来源：http://dqm.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://yri.dianchejie.cn

C#:   e.Message;  e.StackTrace
来源：http://fvs.jqgufenzy.top

[H09] 带错误码的异常
来源：http://yny.daxiang520.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://swb.hesvh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rjw.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aho.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://koz.wangdashe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kjm.hywenlv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kfn.jianghu66.top

Ruby: raise MyError.new("fail", 500)
来源：http://spq.epnwcf.com

C#:   // 自定义异常类中加 Code 属性
来源：http://xuz.dashuyun.cn

[H10] 资源自动释放
来源：http://nhe.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lwl.guowangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jkx.zhiwuduotai.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sjf.ppjwa.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ikx.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cdi.dianchejie.cn

Go:   defer f.Close()
来源：http://sqt.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qjx.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wmx.zhixingplan.top

================================================================================
来源：http://tkl.hammf.cn

I. 正则表达式
来源：http://fqw.svipenyu.cn

================================================================================
来源：http://biw.zycfv.cn

[I01] 判断是否匹配
来源：http://eao.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nyu.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://khv.fehbvm.com

JS:   /\d+/.test(s)
来源：http://oxz.zhoulong.xyz

TS:   /\d+/.test(s)
来源：http://lpa.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://snl.daria6918.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bhf.ctjpmb.com

Ruby: s.match?(/\d+/)
来源：http://vnf.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eov.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://efz.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://afl.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://syz.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://snt.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://vzq.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tpm.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yol.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://ruh.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fte.gogol.net.cn

[I03] 提取捕获分组
来源：http://nog.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uju.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kab.ydzc1.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jue.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bxt.hammf.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lic.pycfn.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yfo.havefunace.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vep.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mzp.ydjk.org.cn

[I04] 正则替换
来源：http://ruj.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://oqr.fktsv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bdo.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hmp.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://lkf.zdbjq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mgg.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://cnz.jiagoushi.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ody.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tzp.xingfuxueyuan.xyz

[I05] 按正则拆分
来源：http://rtg.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://obc.aibaodan.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yab.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://pgi.zhaomingkeji.xyz

TS:   s.split(/\s*,\s*/)
来源：http://veq.cashguo.top

Java: s.split("\\s*,\\s*")
来源：http://jwq.0kj1m.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ksr.havefunace.top

Ruby: s.split(/\s*,\s*/)
来源：http://gzu.hammf.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://opr.jiagoushi.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ega.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qqh.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hpb.kuanghao11.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kma.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ble.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dkx.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ycc.feifeiyinyue.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aha.iojbl.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rou.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://qga.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ify.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://exe.hesvh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vdc.daria6918.cn

TS:   /error/gim
来源：http://ymv.ywan-chungtsiang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xoj.iojbl.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iao.tianlin.xyz

Ruby: s.scan(/error/i)
来源：http://bvd.meibo888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://had.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://sha.zhongyouzk.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pux.bbcook.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fhe.wangshuangyany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kor.ybcxt.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://brv.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://rdi.yueranfly.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://frs.yongpay.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qaq.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bmc.dashuyun.cn

================================================================================
来源：http://ees.zhongyouzk.top

J. 日期与时间
来源：http://igy.0kj1m.cn

================================================================================
来源：http://edf.yvedp.cn

[J01] 获取当前时间
来源：http://dfz.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wxj.snrcjt.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hmv.jianghu66.top

JS:   new Date();  Date.now()
来源：http://jwj.gaohongyu789.top

TS:   new Date();  Date.now()
来源：http://qli.jiagoushi.top

Java: LocalDateTime.now();  Instant.now()
来源：http://syt.shzxlz.cn

Go:   time.Now()
来源：http://vda.yonumen.top

Ruby: Time.now
来源：http://wiz.chenzaomai.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kih.zhengqikj.top

[J02] 格式化输出
来源：http://tli.sjlbkw.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jlp.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wpg.yonumen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nrk.daxiang520.top

TS:   d.toISOString()
来源：http://roe.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kyb.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pih.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fzq.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qkd.nanxuanxn.top

[J03] 字符串解析为日期
来源：http://hhl.havefunace.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sjo.fengsongda.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zak.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://vaf.yanxiufei.cn

TS:   new Date("2024-01-02")
来源：http://qbu.cdnleiting.top

Java: LocalDate.parse("2024-01-02")
来源：http://zzb.tanke756.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ato.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://yly.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ube.redwolf501.top

[J04] 时间戳与日期互转
来源：http://iid.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xiw.yfazqb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zyw.uphjek.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ncv.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ifp.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qnv.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pun.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://saa.yvedp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tyo.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://mlo.yj20258.top

Py:   now + timedelta(days=7)
来源：http://bnk.zhiwuduotai.top


<!-- 参考信息 -->