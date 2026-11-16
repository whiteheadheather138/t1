代发 wailian999

TS:   public / protected / private
来源：http://wdn.zdqjudy.top

Java: public / protected / private / 默认包级
来源：http://nla.shanyushiyangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bco.daxiang520.top

Ruby: public / protected / private
来源：http://ppu.sufxvd.cn

C#:   public / protected / private / internal
来源：http://czc.0kj1m.cn

[G11] getter / setter
来源：http://row.fzhhl.top

Py:   @property 与 @x.setter
来源：http://xhl.ydzc1.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kiy.ppjwa.cn

JS:   get name() { return this._name; }
来源：http://wao.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://god.uphjek.com

Java: public String getName() { return name; }
来源：http://uln.ivvv.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://dun.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://mty.zhiwuduotai.top

[G12] 对象转字符串
来源：http://kxp.tarul.cn

Py:   def __str__(self): return self.name
来源：http://xmo.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dqx.yangfankeji.com

JS:   toString() { return this.name; }
来源：http://jur.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://jce.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://joi.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nop.yueranfly.top

Ruby: def to_s; @name; end
来源：http://wrw.yj20258.top

C#:   public override string ToString() => Name;
来源：http://blm.gogol.net.cn

[G13] 判断对象类型
来源：http://ptb.zhaomingkeji.xyz

Py:   isinstance(u, User)
来源：http://giw.jqgufenzy.top

PHP:  $u instanceof User
来源：http://heq.ppjwa.cn

JS:   u instanceof User
来源：http://mki.iojbl.cn

TS:   u instanceof User
来源：http://pun.birdmap.top

Java: u instanceof User
来源：http://yfx.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://uhw.sxryk.cn

Ruby: u.is_a?(User)
来源：http://kbo.smart0.xyz

C#:   u is User
来源：http://otm.aizwys.cn

[G14] 数据类 / record
来源：http://ort.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rcm.ctjpmb.com

PHP:  // 用 readonly 属性模拟
来源：http://znv.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://rlg.zdbjq.cn

TS:   type User = { name: string; age: number };
来源：http://oen.fehbvm.com

Java: record User(String name, int age) {}
来源：http://cbh.chenjidiqi.icu

Go:   type User struct { Name string; Age int }
来源：http://sbi.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rnv.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://fdo.haohaochexian.top

[G15] 枚举
来源：http://aam.yangfankeji.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hvh.jyoumei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://icy.hfpthk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bsm.svipenyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fxv.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://soq.daxiang520.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rev.daxiang520.top

Ruby: Color = %i[red green].freeze
来源：http://bno.daxiang520.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yzr.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://drp.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mkv.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://pmn.zhijiandao.cn

JS:   Object.entries(obj)
来源：http://uqr.svipenyu.cn

TS:   Object.entries(obj)
来源：http://yti.guowangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rtz.c1oappe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dil.vqdsnc.cn

Ruby: obj.instance_variables
来源：http://gst.shangyingyoupin.top

C#:   // 用反射或 System.Text.Json
来源：http://jls.xuetiantiany.cn

================================================================================
来源：http://ekm.sjlbkw.cn

H. 异常与错误处理
来源：http://kcq.jinyuanbaomall.cn

================================================================================
来源：http://fcq.ppjwa.cn

[H01] try / catch 基础
来源：http://iuc.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vnh.sxryk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xjl.aibaodan.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ccj.kuanghao11.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xec.52xcode.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yff.daria6918.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lyb.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cmt.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zjn.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://tvs.zdqjudy.top

Py:   try: f()⏎finally: cleanup()
来源：http://mkg.jyoumei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yrm.hywenlv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://igg.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uty.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://ekm.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gva.cqqwz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xmt.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mte.hfpthk.cn

[H03] 主动抛出异常
来源：http://lbe.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://zwe.hesvh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yby.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://vtq.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://qnh.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ysv.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://upd.zhiwuduotai.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cgk.andypj.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://zml.yueranfly.top

[H04] 自定义异常类型
来源：http://dam.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://gmf.jinqigfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://tks.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://tri.pengpengdd.cyou

TS:   class MyError extends Error {}
来源：http://lpz.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://qmo.shanyushiyangtech.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kmz.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://vcj.sufxvd.cn

C#:   class MyException : Exception {}
来源：http://uoi.zdqjudy.top

[H05] 捕获特定类型
来源：http://ntv.zhongyouzk.top

Py:   except ValueError as e:
来源：http://qik.52xcode.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lrn.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://qgq.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://drw.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://fct.epnwcf.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mlf.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://jyk.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vqd.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://htx.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://scb.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gxa.sysykeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://tnk.yfazqb.com

TS:   obj?.a?.b;  d ?? default
来源：http://zjs.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jll.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mqo.nwbrower.top

Ruby: d&.dig(:a, :b)
来源：http://gcm.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://myq.aizwys.cn

[H07] 断言
来源：http://qwt.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://bbx.0kj1m.cn

PHP:  assert($x > 0);
来源：http://yos.yj202588.top

JS:   console.assert(x > 0);
来源：http://umq.birdmap.top

TS:   console.assert(x > 0);
来源：http://ohh.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://oyi.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rnn.hcnkem.com

Ruby: raise "必须为正" unless x > 0
来源：http://ffd.vqdsnc.cn

C#:   Debug.Assert(x > 0);
来源：http://oza.yongpay.top

[H08] 获取错误信息与堆栈
来源：http://qcl.fanxiaobao.xyz

Py:   str(e);  traceback.format_exc()
来源：http://jwb.hnqzz.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tuc.svipenyu.cn

JS:   e.message;  e.stack
来源：http://yyx.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lky.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pdn.gogol.net.cn

Go:   err.Error()
来源：http://jsg.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://fwm.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://jpa.haohaochexian.top

[H09] 带错误码的异常
来源：http://ypk.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gef.0kj1m.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oiw.yj20258.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jiw.mhx1999.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://liy.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kzj.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zol.hnqzz.top

Ruby: raise MyError.new("fail", 500)
来源：http://wwc.dianchejie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dgz.wangdashe.top

[H10] 资源自动释放
来源：http://kwf.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://jra.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://njk.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rlg.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ewg.cheryme.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cah.ivvv.top

Go:   defer f.Close()
来源：http://pyi.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ssp.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eyj.zhijiandao.cn

================================================================================
来源：http://yfw.cashguo.top

I. 正则表达式
来源：http://tzt.sysykeji.top

================================================================================
来源：http://gva.ctjpmb.com

[I01] 判断是否匹配
来源：http://ysa.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mdm.ehwqpu.com

PHP:  preg_match('/\d+/', $s);
来源：http://wsv.ybcxt.top

JS:   /\d+/.test(s)
来源：http://fjq.ctjpmb.com

TS:   /\d+/.test(s)
来源：http://xal.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zms.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xty.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://rhi.gzhubu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://igm.daria6918.cn

[I02] 提取所有匹配
来源：http://ads.zhengqikj.top

Py:   re.findall(r"\d+", s)
来源：http://hpo.ydjk.org.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://syi.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bts.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://sdy.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aeq.yj20258.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cco.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://zdi.jqgfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rxk.yanxiufei.cn

[I03] 提取捕获分组
来源：http://bfe.haohaochexian.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yky.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uwu.c1oappe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://afu.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hms.yueranfly.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iyf.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ixf.ivvv.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://trf.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ekq.zhaomingkeji.xyz

[I04] 正则替换
来源：http://iwo.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lum.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hqu.jinghuilouyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mbu.ppjwa.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rgl.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://pzs.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://oxz.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tek.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uwh.fanxiaobao.xyz

[I05] 按正则拆分
来源：http://psj.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://xlv.daria6918.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ovi.ehwqpu.com

JS:   s.split(/\s*,\s*/)
来源：http://xou.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://pxb.hnqzz.top

Java: s.split("\\s*,\\s*")
来源：http://cfl.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dlz.zhijiandao.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zab.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mdc.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://znq.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qil.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jno.zhoulong.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cbz.9152youxi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kud.guowangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xuq.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dxu.wangshuangyany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eit.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ymd.yuxming.cn

[I07] 忽略大小写与多行模式
来源：http://vbk.ydzc1.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gsx.fanxiaobao.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://big.zhiwuduotai.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://syd.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://sxg.zhongyouzk.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oro.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uxs.xuetiantiany.cn

Ruby: s.scan(/error/i)
来源：http://djn.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://znv.fehbvm.com

[I08] 贪婪与非贪婪匹配
来源：http://qnh.ydjk.org.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mmq.cucudq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wfu.sweek.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oxu.zhixingplan.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ldh.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://phu.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dkj.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://owj.bbcook.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lgc.ybcxt.top

================================================================================
来源：http://niw.yj202588.top

J. 日期与时间
来源：http://juw.uphjek.com

================================================================================
来源：http://vqh.epnwcf.com

[J01] 获取当前时间
来源：http://uwo.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://meh.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://olq.daria6918.cn

JS:   new Date();  Date.now()
来源：http://kjd.gzhubu.top

TS:   new Date();  Date.now()
来源：http://bbd.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hdk.vehdjk.com

Go:   time.Now()
来源：http://kcz.xylfe.cn

Ruby: Time.now
来源：http://mpe.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hdf.zycfv.cn

[J02] 格式化输出
来源：http://der.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pjy.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hsj.nanxuanxn.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://llv.birdmap.top

TS:   d.toISOString()
来源：http://dnm.yvedp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tju.cucudq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fbm.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://geo.zdbjq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dup.wangshuangyany.cn

[J03] 字符串解析为日期
来源：http://pjs.0kj1m.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qby.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fdw.yueranfly.top

JS:   new Date("2024-01-02")
来源：http://oyr.ivvv.top

TS:   new Date("2024-01-02")
来源：http://sqw.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://xny.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tsj.tianlin.xyz

Ruby: Date.parse("2024-01-02")
来源：http://dif.ywan-chungtsiang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ecw.hnxiangtu.top

[J04] 时间戳与日期互转
来源：http://aak.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zog.hesvh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wki.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gbr.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://bik.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gwh.jiagoushi.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tmr.jyoumei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xbf.yuanzhike.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rbi.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://jyl.zhoulong.xyz

Py:   now + timedelta(days=7)
来源：http://cgl.jqgfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wkr.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://med.cdnleiting.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xqy.jinqigfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://pja.zycfv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uei.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://nke.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://vbt.ydzc1.top

[J06] 计算两时间之差
来源：http://bhd.tianlin.xyz

Py:   (end - start).total_seconds()
来源：http://okh.quarkkingdee.top

PHP:  $end->diff($start)->days;
来源：http://gbw.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://apk.yuanzhike.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xpf.zycfv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://joh.zhijiandao.cn

Go:   end.Sub(start).Hours()
来源：http://omp.ctjpmb.com

Ruby: end - start                 # 返回秒数
来源：http://xyu.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://ctm.havefunace.top

[J07] 比较两个日期
来源：http://nam.tanke756.top

Py:   d1 < d2;  d1 == d2
来源：http://rwn.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zsx.shuidangran.top

JS:   d1.getTime() < d2.getTime()
来源：http://vrq.shangyingyoupin.top

TS:   d1.getTime() < d2.getTime()
来源：http://gnl.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rus.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hzi.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://rjk.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://ecj.fzhhl.top

[J08] 提取年月日与星期
来源：http://svq.shanyushiyangtech.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://npl.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://arr.sxryk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jva.guannengcc.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xtg.yanxiufei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ibt.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jgs.shuidangran.top


<!-- 参考信息 -->