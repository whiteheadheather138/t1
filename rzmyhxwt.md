代发 wailian999

Ruby: super
来源：http://sra.xziqi.cn

C#:   base.Greet();
来源：http://wje.zhoulong.xyz

[G08] 静态方法与属性
来源：http://zrm.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kbm.yangfankeji.com

PHP:  public static function f() {}
来源：http://lyw.cheryme.top

JS:   static f() {}
来源：http://adv.vqdsnc.cn

TS:   static f(): void {}
来源：http://nqj.jinqigufen.top

Java: static void f() {}
来源：http://qnl.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bdj.ybcxt.top

Ruby: def self.f; end
来源：http://apf.svipenyu.cn

C#:   public static void F() {}
来源：http://hnw.xuetiantiany.cn

[G09] 接口 / 抽象类
来源：http://ahs.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://awu.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jrv.xziqi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://joo.yongpay.top

TS:   interface Shape { area(): number; }
来源：http://krh.ivvv.top

Java: interface Shape { double area(); }
来源：http://guz.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://fmb.gzhubu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xka.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://qfn.redwolf501.top

[G10] 访问控制
来源：http://zdr.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://nzr.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://dbk.havefunace.top

JS:   #private 字段；其余公开
来源：http://zgg.xuetiantiany.cn

TS:   public / protected / private
来源：http://qsv.zhaomingkeji.xyz

Java: public / protected / private / 默认包级
来源：http://mdc.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ywa.xuanzx.com

Ruby: public / protected / private
来源：http://hzw.hysaishi.cn

C#:   public / protected / private / internal
来源：http://bfm.ehwqpu.com

[G11] getter / setter
来源：http://vrt.316326.xyz

Py:   @property 与 @x.setter
来源：http://fij.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xmb.jqgfzy.top

JS:   get name() { return this._name; }
来源：http://jjd.cqqwz.cn

TS:   get name(): string { return this._name; }
来源：http://ezl.pycfn.com

Java: public String getName() { return name; }
来源：http://cge.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://igy.zhiwuduotai.top

Ruby: attr_accessor :name
来源：http://ynp.sweek.top

C#:   public string Name { get; set; }
来源：http://ktw.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://rpx.yj202588.top

Py:   def __str__(self): return self.name
来源：http://eps.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zzd.yj20258888.top

JS:   toString() { return this.name; }
来源：http://kvn.ivvv.top

TS:   toString(): string { return this.name; }
来源：http://uvb.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://zbm.yangfankeji.com

Go:   func (u User) String() string { return u.Name }
来源：http://clq.sufxvd.cn

Ruby: def to_s; @name; end
来源：http://hwo.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://vqi.nanxinkj.top

[G13] 判断对象类型
来源：http://wsj.daria6918.cn

Py:   isinstance(u, User)
来源：http://dfc.ppjwa.cn

PHP:  $u instanceof User
来源：http://nju.nanxuanxn.top

JS:   u instanceof User
来源：http://ufg.aibaodan.cn

TS:   u instanceof User
来源：http://bhu.guannengcc.top

Java: u instanceof User
来源：http://lbk.xuanzx.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://dpk.guannengcc.top

Ruby: u.is_a?(User)
来源：http://fgo.zhiwuduotai.top

C#:   u is User
来源：http://eqn.fktsv.cn

[G14] 数据类 / record
来源：http://ubz.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bgp.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://zux.shzxlz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xyb.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://drj.shanyushiyangkeji.top

Java: record User(String name, int age) {}
来源：http://viy.hesvh.cn

Go:   type User struct { Name string; Age int }
来源：http://qhg.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qxr.sweek.top

C#:   record User(string Name, int Age);
来源：http://dyn.zhijiandao.cn

[G15] 枚举
来源：http://fiu.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gmm.cdnleiting.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pjf.ctjpmb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xwm.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uib.hongshengwenyu.top

Java: enum Color { RED, GREEN }
来源：http://fzx.tianlin.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://odr.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://lbj.feifeiyinyue.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rfw.nanxuanxn.top

[G16] 对象转数组 / 字典
来源：http://zga.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pbh.iojbl.cn

PHP:  get_object_vars($obj);
来源：http://xii.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://awe.yj20258.top

TS:   Object.entries(obj)
来源：http://wne.jinqigfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://skw.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jdf.yonumen.top

Ruby: obj.instance_variables
来源：http://htg.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://qvd.shuidangran.top

================================================================================
来源：http://vcq.hysaishi.cn

H. 异常与错误处理
来源：http://ahj.zhengqikj.top

================================================================================
来源：http://ffo.xingfuxueyuan.xyz

[H01] try / catch 基础
来源：http://ljk.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://muu.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nab.fanxiaobao.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ybk.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rqt.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kke.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dzi.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yss.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mzt.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://vnp.yfazqb.com

Py:   try: f()⏎finally: cleanup()
来源：http://jdt.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uje.sweek.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xxa.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dto.yuxming.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cjq.dianchejie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jct.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rad.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tmg.0kj1m.cn

[H03] 主动抛出异常
来源：http://tez.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://nwu.shanyushiyangtech.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kwm.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://ezm.yangfankeji.com

TS:   throw new Error("错误信息");
来源：http://dcf.daria6918.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mvh.jianghu66.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dea.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zmt.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lzz.hysaishi.cn

[H04] 自定义异常类型
来源：http://zro.bbcook.cn

Py:   class MyError(Exception): pass
来源：http://bji.shzxlz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ylk.nanxinkj.top

JS:   class MyError extends Error {}
来源：http://jmn.jinqigfzy.top

TS:   class MyError extends Error {}
来源：http://hbe.hysaishi.cn

Java: class MyException extends RuntimeException {}
来源：http://apw.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fpn.zhijiandao.cn

Ruby: class MyError < StandardError; end
来源：http://lkx.hysaishi.cn

C#:   class MyException : Exception {}
来源：http://wnv.jianghu66.top

[H05] 捕获特定类型
来源：http://flf.hesvh.cn

Py:   except ValueError as e:
来源：http://qdt.jlsjyb.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tba.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://hch.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://bma.tanke756.top

Java: catch (IOException | SQLException e) {}
来源：http://zwy.gaohongyu789.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qem.shanyushiyangkeji.top

Ruby: rescue ArgumentError => e
来源：http://nys.vqdsnc.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hpi.daxiang520.top

[H06] 可选值 / 空值安全访问
来源：http://iho.daxiang520.top

Py:   value = d.get("k") or default
来源：http://exk.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://cqu.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://mnq.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xec.cheryme.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://abq.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bba.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://atl.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://noa.daxiang520.top

[H07] 断言
来源：http://non.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://uew.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://jxh.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://vxm.jianghu66.top

TS:   console.assert(x > 0);
来源：http://mng.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://vex.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ncg.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vjz.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://hpp.sysykeji.top

[H08] 获取错误信息与堆栈
来源：http://fer.hnxiangtu.top

Py:   str(e);  traceback.format_exc()
来源：http://mja.svipenyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wsi.snrcjt.cn

JS:   e.message;  e.stack
来源：http://yxv.gotoacloud.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kmr.hcnkem.com

Java: e.getMessage();  e.printStackTrace()
来源：http://yii.jiagoushi.top

Go:   err.Error()
来源：http://xli.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://dvj.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://pjw.jinqigufen.top

[H09] 带错误码的异常
来源：http://zkc.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uvy.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cet.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fri.sweek.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sko.hnqzz.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pka.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://swj.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oug.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rht.quarkkingdee.top

[H10] 资源自动释放
来源：http://coh.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jbk.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ile.dashuyun.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://siy.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cqb.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tkv.jqgfzy.top

Go:   defer f.Close()
来源：http://jxx.epnwcf.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://squ.shangyingyoupin.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ppy.zhoulong.xyz

================================================================================
来源：http://zhu.sjlbkw.cn

I. 正则表达式
来源：http://hxh.meibo888.top

================================================================================
来源：http://red.sweek.top

[I01] 判断是否匹配
来源：http://erm.guowangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jei.jinghuilouyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uho.bjfxy.top

JS:   /\d+/.test(s)
来源：http://hfx.jianghu66.top

TS:   /\d+/.test(s)
来源：http://iqd.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sia.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://czl.pengpengdd.cyou

Ruby: s.match?(/\d+/)
来源：http://jme.jlsjyb.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yhc.fanxiaobao.xyz

[I02] 提取所有匹配
来源：http://tkx.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://gyh.hywenlv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oxn.cqqwz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iac.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://qmh.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://doe.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xst.zhoulong.xyz

Ruby: s.scan(/\d+/)
来源：http://npa.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ylm.wangdashe.top

[I03] 提取捕获分组
来源：http://hjd.hysaishi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://smb.yangfankeji.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dnj.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bzd.hfpthk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pvz.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yip.yj20258888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gvn.chenlongwang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pka.yongpay.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sdp.tanke756.top

[I04] 正则替换
来源：http://qbx.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hbw.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sga.jqgufenzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://jwd.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://eov.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://ots.cheryme.top

Go:   re.ReplaceAllString(s, "#")
来源：http://npx.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vjy.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jam.andypj.xyz

[I05] 按正则拆分
来源：http://ezu.xinyue.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://hin.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://emz.fzhhl.top

JS:   s.split(/\s*,\s*/)
来源：http://qzz.xziqi.cn

TS:   s.split(/\s*,\s*/)
来源：http://igr.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://don.hammf.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lzk.fzhhl.top

Ruby: s.split(/\s*,\s*/)
来源：http://adl.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fsz.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eaw.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ewi.xziqi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zgp.sufxvd.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hxe.yanxiufei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xuf.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iic.tarul.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://trx.uphjek.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ujm.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kbw.zhaomingkeji.xyz

[I07] 忽略大小写与多行模式
来源：http://hxq.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://psw.wangdashe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yob.zycfv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ana.zdqjudy.top

TS:   /error/gim
来源：http://jqm.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tkq.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qva.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://dgr.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yra.gaohongyu789.top

[I08] 贪婪与非贪婪匹配
来源：http://gkr.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ocz.hysaishi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hxh.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tzf.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dmo.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yoc.jinqigfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://azw.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mpx.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qks.guowangkeji.top

================================================================================
来源：http://liy.shanyushiyangtech.top

J. 日期与时间
来源：http://kcg.hysaishi.cn

================================================================================
来源：http://sbn.havefunace.top

[J01] 获取当前时间
来源：http://mmp.mhx1999.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ybm.9152youxi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ago.aibaodan.cn

JS:   new Date();  Date.now()
来源：http://ksu.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://bde.xinyue.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://dvt.fktsv.cn

Go:   time.Now()
来源：http://beg.jiagoushi.top

Ruby: Time.now
来源：http://dow.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nie.bjfxy.top

[J02] 格式化输出
来源：http://ddr.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rvh.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://try.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://exj.cqqwz.cn

TS:   d.toISOString()
来源：http://vrj.jinyuanbaomall.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ozq.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rbi.feifeiyinyue.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://imo.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gba.9152youxi.cn

[J03] 字符串解析为日期
来源：http://bey.kuanghao11.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ytj.gotoacloud.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dbz.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://qqm.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://why.yueranfly.top

Java: LocalDate.parse("2024-01-02")
来源：http://xal.guannengcc.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mai.jlsjyb.cn

Ruby: Date.parse("2024-01-02")
来源：http://tnr.vehdjk.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ihk.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://vjp.hammf.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cld.cqqwz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qnr.9152youxi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://slw.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zbj.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://twy.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pmt.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iij.yanxiufei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://azd.gzhubu.top

[J05] 时间加减（加 7 天）
来源：http://rcu.daria6918.cn

Py:   now + timedelta(days=7)
来源：http://xjx.yanxiufei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vgb.9152youxi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iyu.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dgp.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://oop.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dcn.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://xic.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://bgd.feifeiyinyue.top

[J06] 计算两时间之差
来源：http://idt.yj20258.top


<!-- 参考信息 -->