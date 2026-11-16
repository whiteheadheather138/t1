代发 wailian999

Java: interface Shape { double area(); }
来源：http://iov.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://vkk.yfazqb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uxk.yj20258.top

C#:   interface IShape { double Area(); }
来源：http://kec.andypj.xyz

[G10] 访问控制
来源：http://vho.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://efl.jinqigfzy.top

PHP:  public / protected / private
来源：http://qeg.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://rin.52xcode.cn

TS:   public / protected / private
来源：http://zjm.zhoulong.xyz

Java: public / protected / private / 默认包级
来源：http://ljs.zdbjq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pqi.wangdashe.top

Ruby: public / protected / private
来源：http://cuh.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://xjp.hcnkem.com

[G11] getter / setter
来源：http://ixp.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://tqx.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ciu.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://ymj.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://hrj.bjfxy.top

Java: public String getName() { return name; }
来源：http://fmy.jinghuilouyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fhq.gotoacloud.top

Ruby: attr_accessor :name
来源：http://owg.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://hvu.dashuyun.cn

[G12] 对象转字符串
来源：http://llk.dianchejie.cn

Py:   def __str__(self): return self.name
来源：http://wnv.hfpthk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dgv.guowangkeji.top

JS:   toString() { return this.name; }
来源：http://qkr.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://xyo.yfazqb.com

Java: @Override public String toString() { return name; }
来源：http://rzy.cheryme.top

Go:   func (u User) String() string { return u.Name }
来源：http://ngp.52xcode.cn

Ruby: def to_s; @name; end
来源：http://qus.fengsongda.top

C#:   public override string ToString() => Name;
来源：http://lih.feifeiyinyue.top

[G13] 判断对象类型
来源：http://dvo.vqdsnc.cn

Py:   isinstance(u, User)
来源：http://ija.hywenlv.cn

PHP:  $u instanceof User
来源：http://iqf.cdnleiting.top

JS:   u instanceof User
来源：http://zun.meibo888.top

TS:   u instanceof User
来源：http://obu.yj20258.top

Java: u instanceof User
来源：http://mvx.xuetiantiany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ltv.iojbl.cn

Ruby: u.is_a?(User)
来源：http://aod.hongshengwenyu.top

C#:   u is User
来源：http://dhp.yuxming.cn

[G14] 数据类 / record
来源：http://xnb.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rqr.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://bpl.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://ayb.redwolf501.top

TS:   type User = { name: string; age: number };
来源：http://uqh.zhengqikj.top

Java: record User(String name, int age) {}
来源：http://kwa.zhongyouzk.top

Go:   type User struct { Name string; Age int }
来源：http://epv.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fhf.chenzaomai.com

C#:   record User(string Name, int Age);
来源：http://daa.feifeiyinyue.top

[G15] 枚举
来源：http://roa.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://omo.zhoulong.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://hau.hammf.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hfk.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wvy.feifeiyinyue.top

Java: enum Color { RED, GREEN }
来源：http://upr.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xcg.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://eqe.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://byv.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://cij.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gvn.nanxuanxn.top

PHP:  get_object_vars($obj);
来源：http://ghh.zhijiandao.cn

JS:   Object.entries(obj)
来源：http://zgr.chenlongwang.top

TS:   Object.entries(obj)
来源：http://ewf.jyoumei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hnm.yanxiufei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ipv.yj202588.top

Ruby: obj.instance_variables
来源：http://hsy.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://kpc.yj20258888.top

================================================================================
来源：http://ymj.gzhubu.top

H. 异常与错误处理
来源：http://qzb.cqqwz.cn

================================================================================
来源：http://zgo.nanxuanxn.top

[H01] try / catch 基础
来源：http://dnp.hnxiangtu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oes.ywan-chungtsiang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xin.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://daz.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rio.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zna.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jss.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qqn.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://llv.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://gfj.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://swp.hcnkem.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://vba.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rvk.tarul.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cgf.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://eyz.ydzc1.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uaq.52xcode.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://csz.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://hxt.sysykeji.top

[H03] 主动抛出异常
来源：http://hun.hywenlv.cn

Py:   raise ValueError("错误信息")
来源：http://qsq.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ruq.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://sgw.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://tor.hysaishi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://umk.cdnleiting.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tfj.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ydd.havefunace.top

C#:   throw new ArgumentException("错误信息");
来源：http://grj.meibo888.top

[H04] 自定义异常类型
来源：http://ngs.mhx1999.top

Py:   class MyError(Exception): pass
来源：http://sfa.xuanzx.com

PHP:  class MyError extends RuntimeException {}
来源：http://qzf.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://kmm.xuanzx.com

TS:   class MyError extends Error {}
来源：http://src.pengpengdd.cyou

Java: class MyException extends RuntimeException {}
来源：http://bse.zhengqikj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bvh.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://oeh.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://nvm.jinyuanbaomall.cn

[H05] 捕获特定类型
来源：http://bbt.epnwcf.com

Py:   except ValueError as e:
来源：http://zis.yangfankeji.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://roo.yuanzhike.top

JS:   if (e instanceof TypeError) {}
来源：http://wjz.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://hxu.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://smu.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nuw.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://use.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kvy.gzhubu.top

[H06] 可选值 / 空值安全访问
来源：http://emg.bbcook.cn

Py:   value = d.get("k") or default
来源：http://lmv.nanxuanxn.top

PHP:  $v = $d["k"] ?? null;
来源：http://oph.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cwk.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://piz.zdqjudy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fcj.chenjidiqi.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://rkm.pengpengdd.cyou

Ruby: d&.dig(:a, :b)
来源：http://jwx.jinyuanbaomall.cn

C#:   obj?.A?.B ?? default
来源：http://ott.ybcxt.top

[H07] 断言
来源：http://ucx.sufxvd.cn

Py:   assert x > 0, "必须为正"
来源：http://msc.cdnleiting.top

PHP:  assert($x > 0);
来源：http://zmz.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://hus.sxryk.cn

TS:   console.assert(x > 0);
来源：http://yfq.nwbrower.top

Java: assert x > 0 : "必须为正";
来源：http://mhv.tianlin.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oej.fehbvm.com

Ruby: raise "必须为正" unless x > 0
来源：http://glq.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://ccz.fengsongda.top

[H08] 获取错误信息与堆栈
来源：http://ntj.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://tdx.kuanghao11.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vou.pengpengdd.cyou

JS:   e.message;  e.stack
来源：http://nfq.gotoacloud.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ypz.nanxuanxn.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uou.nwbrower.top

Go:   err.Error()
来源：http://xwp.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://xvn.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://jdt.yonumen.top

[H09] 带错误码的异常
来源：http://fxl.316326.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lba.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mog.redwolf501.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dls.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lqn.gogol.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xdr.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zgm.0kj1m.cn

Ruby: raise MyError.new("fail", 500)
来源：http://aoi.zdbjq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://faj.shangyingyoupin.top

[H10] 资源自动释放
来源：http://ytr.jqgfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wzp.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gpa.cdnleiting.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eea.cdnleiting.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nge.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tiq.sjlbkw.cn

Go:   defer f.Close()
来源：http://cje.smart0.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ppc.hnxiangtu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ygq.kuanghao11.cn

================================================================================
来源：http://pug.vehdjk.com

I. 正则表达式
来源：http://jxd.shanyushiyangkeji.top

================================================================================
来源：http://wjk.shanyushiyangkeji.top

[I01] 判断是否匹配
来源：http://biw.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mxt.bjfxy.top

PHP:  preg_match('/\d+/', $s);
来源：http://rwm.bbcook.cn

JS:   /\d+/.test(s)
来源：http://xxn.zhoulong.xyz

TS:   /\d+/.test(s)
来源：http://drw.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oog.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tdc.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://gqj.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://btl.zhoulong.xyz

[I02] 提取所有匹配
来源：http://oiz.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://hcp.vqdsnc.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ayp.nanxinkj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aqd.tarul.cn

TS:   s.match(/\d+/g)
来源：http://rgp.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mny.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mjs.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://ijz.yongpay.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iqb.svipenyu.cn

[I03] 提取捕获分组
来源：http://uzt.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ihc.zhongyouzk.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zny.fanxiaobao.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uqk.sweek.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kgv.andypj.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jkp.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ewh.gogol.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qqx.sweek.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rzx.sysykeji.top

[I04] 正则替换
来源：http://tkg.cdnleiting.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vrc.guannengcc.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://axs.vqdsnc.cn

JS:   s.replace(/\d+/g, "#")
来源：http://toq.mhx1999.top

TS:   s.replace(/\d+/g, "#")
来源：http://swu.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cya.guowangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tvd.zhijiandao.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pdd.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vew.zhengqikj.top

[I05] 按正则拆分
来源：http://xsh.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xos.pengpengdd.cyou

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bar.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://zdb.jianghu66.top

TS:   s.split(/\s*,\s*/)
来源：http://rvk.zhiwuduotai.top

Java: s.split("\\s*,\\s*")
来源：http://pzf.9152youxi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lmq.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://krx.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lgr.yj20258.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yui.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lez.mhx1999.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nuk.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vir.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mdu.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ubf.tarul.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://syy.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hjp.yvedp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lfg.tian-w.cn

[I07] 忽略大小写与多行模式
来源：http://zaj.quarkkingdee.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mcv.kuanghao11.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hxb.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cxe.chenlongwang.top

TS:   /error/gim
来源：http://kne.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eag.jinqigfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://flb.xziqi.cn

Ruby: s.scan(/error/i)
来源：http://epw.zycfv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fop.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://oex.chenjidiqi.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hnl.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://szj.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wbl.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vce.daria6918.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://btx.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ktf.yonumen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ivi.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cjk.zhijiandao.cn

================================================================================
来源：http://nhu.xinyue.icu

J. 日期与时间
来源：http://zkv.hysaishi.cn

================================================================================
来源：http://ohd.feifeiyinyue.top

[J01] 获取当前时间
来源：http://ilx.wangdashe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rmf.ywan-chungtsiang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iam.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://urx.yj202588.top

TS:   new Date();  Date.now()
来源：http://ybg.havefunace.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uro.sjlbkw.cn

Go:   time.Now()
来源：http://phj.cashguo.top

Ruby: Time.now
来源：http://keg.ctjpmb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qlg.yvedp.cn

[J02] 格式化输出
来源：http://jdk.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zwp.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://odx.nanxinkj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gnd.pengpengdd.cyou

TS:   d.toISOString()
来源：http://vbw.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kmx.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fpo.vqdsnc.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rjn.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wnk.shuidangran.top

[J03] 字符串解析为日期
来源：http://uvq.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xaw.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qqz.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://tim.tanke756.top

TS:   new Date("2024-01-02")
来源：http://yft.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://ort.316326.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jtt.fktsv.cn

Ruby: Date.parse("2024-01-02")
来源：http://tnd.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cjz.bjfxy.top

[J04] 时间戳与日期互转
来源：http://knr.gaohongyu789.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ubq.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eca.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rkg.jiagoushi.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xsj.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ryg.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tto.jinqigufen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cla.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bzd.bjfxy.top

[J05] 时间加减（加 7 天）
来源：http://rob.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://nlj.nanxinkj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ryo.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://enx.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yap.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://bka.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pvn.yj20258888.top

Ruby: Time.now + 7 * 86400
来源：http://kch.cashguo.top

C#:   DateTime.Now.AddDays(7)
来源：http://mmw.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://zhh.zhiwuduotai.top

Py:   (end - start).total_seconds()
来源：http://srd.zdqjudy.top

PHP:  $end->diff($start)->days;
来源：http://kru.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nga.yueranfly.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wut.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://taq.fanxiaobao.xyz

Go:   end.Sub(start).Hours()
来源：http://xls.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://rim.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://hlu.jqgufenzy.top

[J07] 比较两个日期
来源：http://nkr.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://mxc.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mzu.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://ypz.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://cyn.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sbi.9152youxi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vfa.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://rly.zhengqikj.top


<!-- 参考信息 -->