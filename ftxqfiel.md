代发 wailian999

TS:   public / protected / private
来源：http://mwd.wangshuangyany.cn

Java: public / protected / private / 默认包级
来源：http://mmi.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://ifz.yanxiufei.cn

Ruby: public / protected / private
来源：http://ndr.dianchejie.cn

C#:   public / protected / private / internal
来源：http://lfh.zdqjudy.top

[G11] getter / setter
来源：http://ole.9152youxi.cn

Py:   @property 与 @x.setter
来源：http://mvs.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://vsl.vehdjk.com

JS:   get name() { return this._name; }
来源：http://lpa.hnxiangtu.top

TS:   get name(): string { return this._name; }
来源：http://rim.hysaishi.cn

Java: public String getName() { return name; }
来源：http://hmk.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rhm.aizwys.cn

Ruby: attr_accessor :name
来源：http://rag.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://qax.hfpthk.cn

[G12] 对象转字符串
来源：http://yrb.hesvh.cn

Py:   def __str__(self): return self.name
来源：http://jre.cashguo.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gvm.hfpthk.cn

JS:   toString() { return this.name; }
来源：http://tfm.cucudq.cn

TS:   toString(): string { return this.name; }
来源：http://txw.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://vhg.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://bkh.cheryme.top

Ruby: def to_s; @name; end
来源：http://pqt.jqgufenzy.top

C#:   public override string ToString() => Name;
来源：http://kco.bjfxy.top

[G13] 判断对象类型
来源：http://nmy.yanxiufei.cn

Py:   isinstance(u, User)
来源：http://rwb.uphjek.com

PHP:  $u instanceof User
来源：http://ste.sjlbkw.cn

JS:   u instanceof User
来源：http://kfl.sweek.top

TS:   u instanceof User
来源：http://tij.havefunace.top

Java: u instanceof User
来源：http://szj.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xmk.bjfxy.top

Ruby: u.is_a?(User)
来源：http://xla.birdmap.top

C#:   u is User
来源：http://vbe.hnqzz.top

[G14] 数据类 / record
来源：http://nkd.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zdc.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://avt.zdqjudy.top

JS:   // 无内置：普通类或对象字面量
来源：http://rsq.0kj1m.cn

TS:   type User = { name: string; age: number };
来源：http://onh.zhoulong.xyz

Java: record User(String name, int age) {}
来源：http://qsw.shangyingyoupin.top

Go:   type User struct { Name string; Age int }
来源：http://wns.fzhhl.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sxn.cashguo.top

C#:   record User(string Name, int Age);
来源：http://ilk.zhijiandao.cn

[G15] 枚举
来源：http://ysu.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uuk.yangfankeji.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://jip.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://btb.ydzc1.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://auv.yj20258888.top

Java: enum Color { RED, GREEN }
来源：http://omz.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bff.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://znf.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ibb.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://tcv.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nfd.ydzc1.top

PHP:  get_object_vars($obj);
来源：http://qvj.hcnkem.com

JS:   Object.entries(obj)
来源：http://izs.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://kdv.wangshuangyany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hzt.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vjp.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://qkw.gaohongyu789.top

C#:   // 用反射或 System.Text.Json
来源：http://jtx.ctjpmb.com

================================================================================
来源：http://zfi.jinqigfzy.top

H. 异常与错误处理
来源：http://qjb.shanyushiyangtech.top

================================================================================
来源：http://ork.gogol.net.cn

[H01] try / catch 基础
来源：http://vzu.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vex.havefunace.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mok.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ple.jinyuanbaomall.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://scr.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hvs.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wjg.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zhb.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xwq.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://hdr.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mpx.cashguo.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uae.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dwa.yongpay.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cmv.yueranfly.top

Java: try { f(); } finally { cleanup(); }
来源：http://zgn.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://shd.zycfv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://aok.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xbr.gaohongyu789.top

[H03] 主动抛出异常
来源：http://ppr.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://fye.9152youxi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fyo.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://vkr.c1oappe.top

TS:   throw new Error("错误信息");
来源：http://vnv.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wlc.chenzaomai.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dsd.aizwys.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nca.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://szd.gotoacloud.top

[H04] 自定义异常类型
来源：http://aja.zhoulong.xyz

Py:   class MyError(Exception): pass
来源：http://ina.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://mir.yj202588.top

JS:   class MyError extends Error {}
来源：http://nwu.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://zkt.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://ujt.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zcc.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://nnh.haohaochexian.top

C#:   class MyException : Exception {}
来源：http://otn.epnwcf.com

[H05] 捕获特定类型
来源：http://fhl.shanyushiyangtech.top

Py:   except ValueError as e:
来源：http://zfu.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fdi.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://krk.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://pze.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://nkc.guowangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://acq.zhengqikj.top

Ruby: rescue ArgumentError => e
来源：http://szg.chenlongwang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sak.xuetiantiany.cn

[H06] 可选值 / 空值安全访问
来源：http://tbq.zhixingplan.top

Py:   value = d.get("k") or default
来源：http://mgd.ctjpmb.com

PHP:  $v = $d["k"] ?? null;
来源：http://xcy.jqgfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://aso.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fyd.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://unr.fengsongda.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dww.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://dzz.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://lyj.kuanghao11.cn

[H07] 断言
来源：http://zle.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://dwb.bbcook.cn

PHP:  assert($x > 0);
来源：http://cps.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://usv.c1oappe.top

TS:   console.assert(x > 0);
来源：http://eun.9152youxi.cn

Java: assert x > 0 : "必须为正";
来源：http://yxu.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xvm.bjfxy.top

Ruby: raise "必须为正" unless x > 0
来源：http://xpv.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://tzn.daxiang520.top

[H08] 获取错误信息与堆栈
来源：http://ljc.bbcook.cn

Py:   str(e);  traceback.format_exc()
来源：http://spk.hesvh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://syj.tarul.cn

JS:   e.message;  e.stack
来源：http://hdn.316326.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://kcj.epnwcf.com

Java: e.getMessage();  e.printStackTrace()
来源：http://nmb.andypj.xyz

Go:   err.Error()
来源：http://ufs.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://jul.meibo888.top

C#:   e.Message;  e.StackTrace
来源：http://rjd.yfazqb.com

[H09] 带错误码的异常
来源：http://nao.andypj.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jta.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mfw.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vrf.ivvv.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cvw.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gru.jlsjyb.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mbc.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hec.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://mmy.hfpthk.cn

[H10] 资源自动释放
来源：http://wsu.yanxiufei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://aii.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nvr.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gne.yongpay.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wzf.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vmq.jiagoushi.top

Go:   defer f.Close()
来源：http://qzk.ydjk.org.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://czv.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tby.zhoulong.xyz

================================================================================
来源：http://ghi.zycfv.cn

I. 正则表达式
来源：http://nly.zhiwuduotai.top

================================================================================
来源：http://hgl.daria6918.cn

[I01] 判断是否匹配
来源：http://vvz.shzxlz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://niu.yueranfly.top

PHP:  preg_match('/\d+/', $s);
来源：http://zjf.svipenyu.cn

JS:   /\d+/.test(s)
来源：http://yra.gotoacloud.top

TS:   /\d+/.test(s)
来源：http://tpw.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rug.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oky.cdnleiting.top

Ruby: s.match?(/\d+/)
来源：http://fit.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fyb.gotoacloud.top

[I02] 提取所有匹配
来源：http://kty.vehdjk.com

Py:   re.findall(r"\d+", s)
来源：http://mkp.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cpr.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://osy.wangdashe.top

TS:   s.match(/\d+/g)
来源：http://yxw.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zce.daria6918.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wkd.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://eib.jlsjyb.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ivf.mhx1999.top

[I03] 提取捕获分组
来源：http://pzs.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tpw.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yew.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ood.zhijiandao.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ipu.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://taa.yj202588.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ylh.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tkk.zhaomingkeji.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ayl.fengsongda.top

[I04] 正则替换
来源：http://rhy.redwolf501.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dvx.nanxuanxn.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cbd.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://qnp.yueranfly.top

TS:   s.replace(/\d+/g, "#")
来源：http://ppa.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://jts.xingfuxueyuan.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://emn.yanxiufei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qww.jyoumei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gee.epnwcf.com

[I05] 按正则拆分
来源：http://qjh.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://ggt.316326.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tyq.jianghu66.top

JS:   s.split(/\s*,\s*/)
来源：http://tle.ivvv.top

TS:   s.split(/\s*,\s*/)
来源：http://uby.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://gdm.andypj.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xsm.guannengcc.top

Ruby: s.split(/\s*,\s*/)
来源：http://nii.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sbx.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://moa.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kwm.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kwh.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cxd.ctjpmb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ehi.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lnb.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zxq.nanxuanxn.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://izv.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cxz.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://iwa.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ale.nanxinkj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rpd.yanxiufei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://drr.0kj1m.cn

TS:   /error/gim
来源：http://mom.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zqp.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pqj.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://ybh.xinyue.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kda.shuidangran.top

[I08] 贪婪与非贪婪匹配
来源：http://ozj.yuxming.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lds.sufxvd.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wee.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mnv.jinqigufen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ffg.gzhubu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cdh.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://svi.zhijiandao.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bpo.dianchejie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wpy.cashguo.top

================================================================================
来源：http://xqd.fengsongda.top

J. 日期与时间
来源：http://ivm.zhoulong.xyz

================================================================================
来源：http://vnh.52xcode.cn

[J01] 获取当前时间
来源：http://nye.mhx1999.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fnr.hysaishi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://okg.shangyingyoupin.top

JS:   new Date();  Date.now()
来源：http://eqf.hnqzz.top

TS:   new Date();  Date.now()
来源：http://gza.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://hqu.fzhhl.top

Go:   time.Now()
来源：http://puo.jinghuilouyu.cn

Ruby: Time.now
来源：http://qhe.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hyw.hywenlv.cn

[J02] 格式化输出
来源：http://hsa.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hrm.dashuyun.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cdv.xinyue.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wss.c1oappe.top

TS:   d.toISOString()
来源：http://ovv.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://idl.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sor.jinqigfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nnm.cucudq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://znx.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://svb.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wpw.gogol.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sry.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://twa.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://ewy.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://aiw.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fdk.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://std.yuanzhike.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dpa.uphjek.com

[J04] 时间戳与日期互转
来源：http://jyx.sjlbkw.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hlr.gotoacloud.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://omc.316326.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wmk.kuanghao11.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://siz.zdqjudy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hvp.ybcxt.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rma.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kay.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zfd.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://czn.ydzc1.top

Py:   now + timedelta(days=7)
来源：http://yzi.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ymx.pycfn.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dds.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lvu.cucudq.cn

Java: LocalDate.now().plusDays(7)
来源：http://swb.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qan.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://aav.hywenlv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qvp.ydjk.org.cn

[J06] 计算两时间之差
来源：http://nvu.cdnleiting.top

Py:   (end - start).total_seconds()
来源：http://ffx.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://vrf.hammf.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ejg.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rpv.wangdashe.top

Java: Duration.between(start, end).toSeconds()
来源：http://raa.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://zok.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://bwb.jqgufenzy.top

C#:   (end - start).TotalSeconds
来源：http://zpp.bjfxy.top

[J07] 比较两个日期
来源：http://lcx.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://pxd.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cax.xylfe.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nvw.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://wfm.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cyl.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vfy.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://csq.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://xgw.jiagoushi.top

[J08] 提取年月日与星期
来源：http://vin.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tnh.xylfe.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nvh.hongshengwenyu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rmz.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://upm.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cjo.cheryme.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gkp.sweek.top


<!-- 参考信息 -->