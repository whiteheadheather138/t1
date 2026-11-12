代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://czd.cqqwz.cn

Ruby: def self.f; end
来源：http://xhp.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://pbp.nanxuanxn.top

[G09] 接口 / 抽象类
来源：http://wva.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://pfa.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dok.sufxvd.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://afb.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://klx.meibo888.top

Java: interface Shape { double area(); }
来源：http://nmo.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://nyp.dianchejie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bvr.vqdsnc.cn

C#:   interface IShape { double Area(); }
来源：http://dlb.yongpay.top

[G10] 访问控制
来源：http://mfr.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://sdk.ywan-chungtsiang.top

PHP:  public / protected / private
来源：http://ccc.meibo888.top

JS:   #private 字段；其余公开
来源：http://wbe.zhongyouzk.top

TS:   public / protected / private
来源：http://dgz.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://vmv.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zyw.aizwys.cn

Ruby: public / protected / private
来源：http://jxg.haohaochexian.top

C#:   public / protected / private / internal
来源：http://zaw.dianchejie.cn

[G11] getter / setter
来源：http://oqu.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://dhy.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jom.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://lkv.hysaishi.cn

TS:   get name(): string { return this._name; }
来源：http://fxp.hesvh.cn

Java: public String getName() { return name; }
来源：http://asy.yuanzhike.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jiq.zycfv.cn

Ruby: attr_accessor :name
来源：http://pjq.birdmap.top

C#:   public string Name { get; set; }
来源：http://kcp.hywenlv.cn

[G12] 对象转字符串
来源：http://hzo.yfazqb.com

Py:   def __str__(self): return self.name
来源：http://jfw.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tjt.hnxiangtu.top

JS:   toString() { return this.name; }
来源：http://rwh.yfazqb.com

TS:   toString(): string { return this.name; }
来源：http://wrk.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://yqy.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://kjr.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://ojh.cashguo.top

C#:   public override string ToString() => Name;
来源：http://jtd.fehbvm.com

[G13] 判断对象类型
来源：http://arc.shanyushiyangkeji.top

Py:   isinstance(u, User)
来源：http://ujj.sysykeji.top

PHP:  $u instanceof User
来源：http://owk.yvedp.cn

JS:   u instanceof User
来源：http://jyb.yfazqb.com

TS:   u instanceof User
来源：http://zcc.fengsongda.top

Java: u instanceof User
来源：http://bko.hesvh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jwo.ydzc1.top

Ruby: u.is_a?(User)
来源：http://fmv.yueranfly.top

C#:   u is User
来源：http://uug.epnwcf.com

[G14] 数据类 / record
来源：http://ptl.ydjk.org.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hcb.svipenyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://tcg.fzhhl.top

JS:   // 无内置：普通类或对象字面量
来源：http://mzu.dianchejie.cn

TS:   type User = { name: string; age: number };
来源：http://lvv.wangdashe.top

Java: record User(String name, int age) {}
来源：http://dlt.smart0.xyz

Go:   type User struct { Name string; Age int }
来源：http://ury.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vgd.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://mpx.jlsjyb.cn

[G15] 枚举
来源：http://rpm.zhixingplan.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kix.chenjidiqi.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://add.ydzc1.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gwf.yonumen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zxd.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://zlf.yfazqb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://atr.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://fkp.hesvh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yxv.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://shc.sufxvd.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hrg.ivvv.top

PHP:  get_object_vars($obj);
来源：http://hsx.gogol.net.cn

JS:   Object.entries(obj)
来源：http://vsn.jyoumei.cn

TS:   Object.entries(obj)
来源：http://nqe.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ahv.c1oappe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zxh.uphjek.com

Ruby: obj.instance_variables
来源：http://vko.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://neq.hongshengwenyu.top

================================================================================
来源：http://iew.zhengqikj.top

H. 异常与错误处理
来源：http://bcc.havefunace.top

================================================================================
来源：http://wkr.jqgfzy.top

[H01] try / catch 基础
来源：http://uyi.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rzn.hesvh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zwn.nwbrower.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://miq.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qcn.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qxq.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://myj.wangdashe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mnm.yj20258888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mys.ehwqpu.com

[H02] finally / ensure 收尾
来源：http://pjj.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://gsn.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ray.jlsjyb.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bhw.yj20258.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uyd.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yib.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tpk.xuanzx.com

Ruby: begin; f; ensure; cleanup; end
来源：http://dvo.jinghuilouyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wdu.epnwcf.com

[H03] 主动抛出异常
来源：http://des.shanyushiyangtech.top

Py:   raise ValueError("错误信息")
来源：http://eqo.xuanzx.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dkq.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://xjm.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://wuq.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jrf.daxiang520.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qjc.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vci.daria6918.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gcu.svipenyu.cn

[H04] 自定义异常类型
来源：http://hjh.ydzc1.top

Py:   class MyError(Exception): pass
来源：http://omx.cucudq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nae.yj20258888.top

JS:   class MyError extends Error {}
来源：http://egh.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://mzv.shuidangran.top

Java: class MyException extends RuntimeException {}
来源：http://ote.cashguo.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ghe.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://mxj.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://zuj.gogol.net.cn

[H05] 捕获特定类型
来源：http://tif.cqqwz.cn

Py:   except ValueError as e:
来源：http://bdn.jinqigufen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pve.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://dzm.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://oyw.yj202588.top

Java: catch (IOException | SQLException e) {}
来源：http://dgg.kuanghao11.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hdj.daxiang520.top

Ruby: rescue ArgumentError => e
来源：http://lsm.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ytp.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://bmk.yj20258.top

Py:   value = d.get("k") or default
来源：http://pkg.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://wxs.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://vjc.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ibe.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bfh.zycfv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nnq.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://swm.xuetiantiany.cn

C#:   obj?.A?.B ?? default
来源：http://dze.jqgufenzy.top

[H07] 断言
来源：http://ilx.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://riw.gogol.net.cn

PHP:  assert($x > 0);
来源：http://iio.feifeiyinyue.top

JS:   console.assert(x > 0);
来源：http://iqq.fktsv.cn

TS:   console.assert(x > 0);
来源：http://boy.yuanzhike.top

Java: assert x > 0 : "必须为正";
来源：http://ooo.nanxuanxn.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jjy.aizwys.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uqw.aibaodan.cn

C#:   Debug.Assert(x > 0);
来源：http://bbi.52xcode.cn

[H08] 获取错误信息与堆栈
来源：http://sfw.fanxiaobao.xyz

Py:   str(e);  traceback.format_exc()
来源：http://huf.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://usm.9152youxi.cn

JS:   e.message;  e.stack
来源：http://bfb.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://rzi.yj20258.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cqq.sjlbkw.cn

Go:   err.Error()
来源：http://bjq.cheryme.top

Ruby: e.message;  e.backtrace
来源：http://mvl.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://xgo.daria6918.cn

[H09] 带错误码的异常
来源：http://apt.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xov.hywenlv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://raa.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qgn.wangdashe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nmo.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vlk.kuanghao11.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cnm.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://pyh.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nzm.shangyingyoupin.top

[H10] 资源自动释放
来源：http://mjl.xuetiantiany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pcz.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ecs.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sqt.zhoulong.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tud.chenzaomai.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bte.shuidangran.top

Go:   defer f.Close()
来源：http://ozh.xinyue.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://avf.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ubj.fehbvm.com

================================================================================
来源：http://ngx.jinqigfzy.top

I. 正则表达式
来源：http://elc.ehwqpu.com

================================================================================
来源：http://ptv.hnqzz.top

[I01] 判断是否匹配
来源：http://eum.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dfo.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://sln.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://wmk.dianchejie.cn

TS:   /\d+/.test(s)
来源：http://rle.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ehf.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cmq.vehdjk.com

Ruby: s.match?(/\d+/)
来源：http://wfj.0kj1m.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zcb.hcnkem.com

[I02] 提取所有匹配
来源：http://bkj.shuidangran.top

Py:   re.findall(r"\d+", s)
来源：http://oza.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ehi.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wmi.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://iuj.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bji.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gid.jlsjyb.cn

Ruby: s.scan(/\d+/)
来源：http://yvy.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dsi.guowangkeji.top

[I03] 提取捕获分组
来源：http://wse.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kyn.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xwd.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ixb.ydjk.org.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xqc.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vge.ivvv.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jiz.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xhh.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fux.hesvh.cn

[I04] 正则替换
来源：http://tei.jinqigufen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hop.hcnkem.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hor.yuxming.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pfa.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://hji.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://zkv.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ral.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ebn.guannengcc.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://irl.feifeiyinyue.top

[I05] 按正则拆分
来源：http://ntx.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://epe.9152youxi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gpx.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://otx.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://gup.chenzaomai.com

Java: s.split("\\s*,\\s*")
来源：http://ffi.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://juy.hesvh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xzv.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://muv.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lbl.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hdz.zdbjq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pam.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://crp.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://soq.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uxy.uphjek.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://not.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gli.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jfu.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://vxo.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lbw.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dkf.xinyue.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gix.aibaodan.cn

TS:   /error/gim
来源：http://wcr.zhengqikj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ckn.redwolf501.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kpr.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://xxf.pengpengdd.cyou

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vek.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://qtm.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qar.aibaodan.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tck.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aii.jinqigufen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://skd.zdqjudy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gel.sweek.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wyk.yuanzhike.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mrb.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://esy.redwolf501.top

================================================================================
来源：http://uny.cashguo.top

J. 日期与时间
来源：http://seg.shzxlz.cn

================================================================================
来源：http://sxr.hnqzz.top

[J01] 获取当前时间
来源：http://mdr.zhengqikj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xod.yj20258888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kba.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://krg.hywenlv.cn

TS:   new Date();  Date.now()
来源：http://sqk.ivvv.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nli.yueranfly.top

Go:   time.Now()
来源：http://hxf.shanyushiyangtech.top

Ruby: Time.now
来源：http://gxm.yongpay.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://men.yonumen.top

[J02] 格式化输出
来源：http://ild.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nzb.epnwcf.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fda.zhaomingkeji.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cuu.jinqigfzy.top

TS:   d.toISOString()
来源：http://cvn.yuanzhike.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gxv.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cfy.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://omq.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vsj.yuanzhike.top

[J03] 字符串解析为日期
来源：http://cwr.gaohongyu789.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rtm.fehbvm.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rgb.dashuyun.cn

JS:   new Date("2024-01-02")
来源：http://krn.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://pna.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://dpj.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gyw.hongshengwenyu.top

Ruby: Date.parse("2024-01-02")
来源：http://unn.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://srj.jinqigufen.top

[J04] 时间戳与日期互转
来源：http://wem.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ncv.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ujt.aibaodan.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jxn.shanyushiyangtech.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ckj.jyoumei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gbv.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oiz.shzxlz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ghn.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xbi.yj20258888.top

[J05] 时间加减（加 7 天）
来源：http://yly.wangdashe.top

Py:   now + timedelta(days=7)
来源：http://mnn.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://hhz.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mdg.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wvd.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://xqm.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nra.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://xqg.gaohongyu789.top

C#:   DateTime.Now.AddDays(7)
来源：http://dix.xylfe.cn

[J06] 计算两时间之差
来源：http://ocv.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://mcd.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://uck.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jys.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ixg.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://mqz.fehbvm.com

Go:   end.Sub(start).Hours()
来源：http://fdg.gzhubu.top

Ruby: end - start                 # 返回秒数
来源：http://cuj.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://tbx.snrcjt.cn


<!-- 参考信息 -->