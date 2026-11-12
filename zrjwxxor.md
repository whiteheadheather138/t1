代发 wailian999

JS:   super.greet();
来源：http://lrk.ydzc1.top

TS:   super.greet();
来源：http://nis.ydjk.org.cn

Java: super.greet();
来源：http://gru.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pkh.yfazqb.com

Ruby: super
来源：http://euy.zhiwuduotai.top

C#:   base.Greet();
来源：http://htg.yuanzhike.top

[G08] 静态方法与属性
来源：http://tkh.zhixingplan.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xfe.haohaochexian.top

PHP:  public static function f() {}
来源：http://ijr.cheryme.top

JS:   static f() {}
来源：http://isd.cashguo.top

TS:   static f(): void {}
来源：http://lnj.pengpengdd.cyou

Java: static void f() {}
来源：http://cgd.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://tkx.jiagoushi.top

Ruby: def self.f; end
来源：http://iym.kuanghao11.cn

C#:   public static void F() {}
来源：http://gaa.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://wti.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://ebk.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://htb.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qyh.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://npo.ctjpmb.com

Java: interface Shape { double area(); }
来源：http://pwa.yfazqb.com

Go:   type Shape interface { Area() float64 }
来源：http://sjy.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uqg.zhengqikj.top

C#:   interface IShape { double Area(); }
来源：http://qtp.yangfankeji.com

[G10] 访问控制
来源：http://xes.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://rke.nanxuanxn.top

PHP:  public / protected / private
来源：http://gls.zhijiandao.cn

JS:   #private 字段；其余公开
来源：http://zaa.chenlongwang.top

TS:   public / protected / private
来源：http://eug.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://uza.fehbvm.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://rac.pycfn.com

Ruby: public / protected / private
来源：http://jkm.yuxming.cn

C#:   public / protected / private / internal
来源：http://rsb.chenjidiqi.icu

[G11] getter / setter
来源：http://pjj.xingfuxueyuan.xyz

Py:   @property 与 @x.setter
来源：http://yqr.epnwcf.com

PHP:  public function getName(): string { return $this->name; }
来源：http://sqk.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://gzn.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://ueb.chenlongwang.top

Java: public String getName() { return name; }
来源：http://apo.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jpk.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://ylu.pycfn.com

C#:   public string Name { get; set; }
来源：http://kie.ehwqpu.com

[G12] 对象转字符串
来源：http://mwv.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://yrr.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ofx.chenjidiqi.icu

JS:   toString() { return this.name; }
来源：http://pzt.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://ycd.sweek.top

Java: @Override public String toString() { return name; }
来源：http://ccs.ctjpmb.com

Go:   func (u User) String() string { return u.Name }
来源：http://sxw.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://tpf.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://cxx.yj202588.top

[G13] 判断对象类型
来源：http://gmg.shuidangran.top

Py:   isinstance(u, User)
来源：http://yvk.hesvh.cn

PHP:  $u instanceof User
来源：http://sfa.ppjwa.cn

JS:   u instanceof User
来源：http://yui.jinghuilouyu.cn

TS:   u instanceof User
来源：http://lbo.shuidangran.top

Java: u instanceof User
来源：http://ror.quarkkingdee.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xqp.ywan-chungtsiang.top

Ruby: u.is_a?(User)
来源：http://xdq.bbcook.cn

C#:   u is User
来源：http://wta.fzhhl.top

[G14] 数据类 / record
来源：http://lym.ppjwa.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://epa.52xcode.cn

PHP:  // 用 readonly 属性模拟
来源：http://tze.zhaomingkeji.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://qno.fanxiaobao.xyz

TS:   type User = { name: string; age: number };
来源：http://qrt.pycfn.com

Java: record User(String name, int age) {}
来源：http://iic.yueranfly.top

Go:   type User struct { Name string; Age int }
来源：http://qnu.tanke756.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tgq.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://ror.jqgufenzy.top

[G15] 枚举
来源：http://sto.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://esm.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://tob.tianlin.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ipm.aibaodan.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://orn.uphjek.com

Java: enum Color { RED, GREEN }
来源：http://rof.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vhp.yuanzhike.top

Ruby: Color = %i[red green].freeze
来源：http://pew.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aav.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://qhb.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ojk.aizwys.cn

PHP:  get_object_vars($obj);
来源：http://snl.epnwcf.com

JS:   Object.entries(obj)
来源：http://yuo.zhaomingkeji.xyz

TS:   Object.entries(obj)
来源：http://etl.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kil.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dic.jlsjyb.cn

Ruby: obj.instance_variables
来源：http://ofm.fengsongda.top

C#:   // 用反射或 System.Text.Json
来源：http://yda.fehbvm.com

================================================================================
来源：http://ctd.vqdsnc.cn

H. 异常与错误处理
来源：http://emv.sufxvd.cn

================================================================================
来源：http://gop.sjlbkw.cn

[H01] try / catch 基础
来源：http://lkq.ppjwa.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wic.fzhhl.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fji.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://myn.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xuo.gotoacloud.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fre.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ric.jqgufenzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ygb.haohaochexian.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rui.hnqzz.top

[H02] finally / ensure 收尾
来源：http://pjl.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://mdz.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nvf.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ndb.cdnleiting.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rak.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://ett.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nhe.ydjk.org.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oda.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hxo.tarul.cn

[H03] 主动抛出异常
来源：http://epe.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://mwh.hesvh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uph.havefunace.top

JS:   throw new Error("错误信息");
来源：http://gsh.jiagoushi.top

TS:   throw new Error("错误信息");
来源：http://syp.52xcode.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://koz.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iej.aizwys.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gyz.yj20258.top

C#:   throw new ArgumentException("错误信息");
来源：http://jfb.ehwqpu.com

[H04] 自定义异常类型
来源：http://eaa.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://riz.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tkg.fzhhl.top

JS:   class MyError extends Error {}
来源：http://qnj.sweek.top

TS:   class MyError extends Error {}
来源：http://udf.smart0.xyz

Java: class MyException extends RuntimeException {}
来源：http://ywd.ehwqpu.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kmj.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://dxb.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://dfx.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://fpv.bjfxy.top

Py:   except ValueError as e:
来源：http://sgw.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zpz.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://tfd.chenzaomai.com

TS:   if (e instanceof TypeError) {}
来源：http://mgw.pengpengdd.cyou

Java: catch (IOException | SQLException e) {}
来源：http://hjr.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ngi.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://krd.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bgi.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://mmg.aizwys.cn

Py:   value = d.get("k") or default
来源：http://cvq.jlsjyb.cn

PHP:  $v = $d["k"] ?? null;
来源：http://toj.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://dsp.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://cej.9152youxi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ydy.jinqigfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rgt.ydzc1.top

Ruby: d&.dig(:a, :b)
来源：http://zua.jianghu66.top

C#:   obj?.A?.B ?? default
来源：http://mji.jyoumei.cn

[H07] 断言
来源：http://neq.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://tae.hesvh.cn

PHP:  assert($x > 0);
来源：http://lqj.guannengcc.top

JS:   console.assert(x > 0);
来源：http://wvn.andypj.xyz

TS:   console.assert(x > 0);
来源：http://bkh.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://bby.nanxuanxn.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://odz.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://jvg.cqqwz.cn

C#:   Debug.Assert(x > 0);
来源：http://qas.yuxming.cn

[H08] 获取错误信息与堆栈
来源：http://ost.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://zhk.ehwqpu.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xrt.bjfxy.top

JS:   e.message;  e.stack
来源：http://wif.dianchejie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mil.smart0.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://hbl.zhoulong.xyz

Go:   err.Error()
来源：http://tlr.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://gut.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://mcq.hysaishi.cn

[H09] 带错误码的异常
来源：http://zqe.gaohongyu789.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vev.bjfxy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lmc.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zyf.aizwys.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rdi.zhoulong.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dhq.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vff.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://evq.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dsu.quarkkingdee.top

[H10] 资源自动释放
来源：http://znu.hnqzz.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ggt.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qkq.ehwqpu.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cuy.hnxiangtu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kbv.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zeo.ctjpmb.com

Go:   defer f.Close()
来源：http://tra.zhixingplan.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ynm.kuanghao11.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mjo.316326.xyz

================================================================================
来源：http://xlf.cucudq.cn

I. 正则表达式
来源：http://nff.daria6918.cn

================================================================================
来源：http://ish.yuxming.cn

[I01] 判断是否匹配
来源：http://tix.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ygd.redwolf501.top

PHP:  preg_match('/\d+/', $s);
来源：http://tzl.guannengcc.top

JS:   /\d+/.test(s)
来源：http://ewv.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://hur.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gtc.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ujn.gzhubu.top

Ruby: s.match?(/\d+/)
来源：http://rju.jinqigufen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mls.hammf.cn

[I02] 提取所有匹配
来源：http://lzh.ywan-chungtsiang.top

Py:   re.findall(r"\d+", s)
来源：http://mip.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lep.jiagoushi.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://drg.yj202588.top

TS:   s.match(/\d+/g)
来源：http://tci.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rlq.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xqq.svipenyu.cn

Ruby: s.scan(/\d+/)
来源：http://gsy.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hic.yangfankeji.com

[I03] 提取捕获分组
来源：http://abi.nanxuanxn.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://egk.yj202588.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mou.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://esk.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wmp.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pyf.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://agq.sjlbkw.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hjx.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bzh.yj202588.top

[I04] 正则替换
来源：http://vwm.jianghu66.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yzd.haohaochexian.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yeq.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://ese.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://iyh.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sta.uphjek.com

Go:   re.ReplaceAllString(s, "#")
来源：http://jnt.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://emq.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cof.xinyue.icu

[I05] 按正则拆分
来源：http://vbb.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dgm.zhaomingkeji.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xzt.yanxiufei.cn

JS:   s.split(/\s*,\s*/)
来源：http://xqn.guowangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://mei.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://vns.jiagoushi.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wdw.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cxa.chenjidiqi.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://amz.jinqigfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://agy.fehbvm.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uag.hongshengwenyu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hux.jqgfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zjv.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://azm.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tec.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cer.xuetiantiany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mdj.hesvh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lxw.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://kvc.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uai.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xdr.epnwcf.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ldd.ppjwa.cn

TS:   /error/gim
来源：http://ltg.ywan-chungtsiang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://egf.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fbc.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://dta.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oxa.sjlbkw.cn

[I08] 贪婪与非贪婪匹配
来源：http://xra.tian-w.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bhq.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bwk.zycfv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bem.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pnb.dianchejie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://liz.yvedp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pfi.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xes.xuanzx.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uyi.hfpthk.cn

================================================================================
来源：http://bre.fanxiaobao.xyz

J. 日期与时间
来源：http://msl.hongshengwenyu.top

================================================================================
来源：http://oyl.xuetiantiany.cn

[J01] 获取当前时间
来源：http://dbl.mhx1999.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://edb.dashuyun.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tgy.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://yaj.xuanzx.com

TS:   new Date();  Date.now()
来源：http://iwn.yonumen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://otk.zhaomingkeji.xyz

Go:   time.Now()
来源：http://zsq.shzxlz.cn

Ruby: Time.now
来源：http://aae.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tha.haohaochexian.top

[J02] 格式化输出
来源：http://nfj.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xdg.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://drb.jinqigfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pfa.zhixingplan.top

TS:   d.toISOString()
来源：http://tvd.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cjx.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uju.gzhubu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lcn.xinyue.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kex.cqqwz.cn

[J03] 字符串解析为日期
来源：http://ltl.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pmd.gzhubu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zco.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://ats.quarkkingdee.top

TS:   new Date("2024-01-02")
来源：http://ypi.jyoumei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zkx.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://scs.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://oei.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ndm.tarul.cn

[J04] 时间戳与日期互转
来源：http://apt.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://upo.cucudq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mrz.gaohongyu789.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tuu.hfpthk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xtv.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://skm.daria6918.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kno.ydjk.org.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wvl.uphjek.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dmo.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://tgm.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://iju.shuidangran.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ljh.zhaomingkeji.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nqi.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://psz.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://ntn.chenzaomai.com


<!-- 参考信息 -->