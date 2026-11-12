代发 wailian999

Ruby: attr_accessor :name
来源：http://xdj.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://sci.tanke756.top

[G12] 对象转字符串
来源：http://gwe.kuanghao11.cn

Py:   def __str__(self): return self.name
来源：http://hwm.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://sso.wangdashe.top

JS:   toString() { return this.name; }
来源：http://wkl.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://ciy.yangfankeji.com

Java: @Override public String toString() { return name; }
来源：http://nic.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://feo.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://pqy.sysykeji.top

C#:   public override string ToString() => Name;
来源：http://sgx.pengpengdd.cyou

[G13] 判断对象类型
来源：http://hyk.wangdashe.top

Py:   isinstance(u, User)
来源：http://rfi.tarul.cn

PHP:  $u instanceof User
来源：http://wwb.ctjpmb.com

JS:   u instanceof User
来源：http://cig.ctjpmb.com

TS:   u instanceof User
来源：http://znv.hongshengwenyu.top

Java: u instanceof User
来源：http://pig.yj202588.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xzd.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://vqc.xuanzx.com

C#:   u is User
来源：http://gvl.fehbvm.com

[G14] 数据类 / record
来源：http://fxs.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://llh.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://ryw.guowangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://ljz.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://apw.c1oappe.top

Java: record User(String name, int age) {}
来源：http://krh.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://sul.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tui.cqqwz.cn

C#:   record User(string Name, int Age);
来源：http://ilz.ppjwa.cn

[G15] 枚举
来源：http://ewv.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zuo.sjlbkw.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kwy.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fro.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ogr.sysykeji.top

Java: enum Color { RED, GREEN }
来源：http://pim.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mvf.zhixingplan.top

Ruby: Color = %i[red green].freeze
来源：http://jnd.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sms.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://ynv.hywenlv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iql.zycfv.cn

PHP:  get_object_vars($obj);
来源：http://byv.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://bui.jlsjyb.cn

TS:   Object.entries(obj)
来源：http://uer.tanke756.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mzu.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://iky.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://mad.fanxiaobao.xyz

C#:   // 用反射或 System.Text.Json
来源：http://nri.quarkkingdee.top

================================================================================
来源：http://ruv.yuanzhike.top

H. 异常与错误处理
来源：http://sia.9152youxi.cn

================================================================================
来源：http://xtu.jqgufenzy.top

[H01] try / catch 基础
来源：http://cdx.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ygr.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ghx.yanxiufei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://phr.gaohongyu789.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rys.daria6918.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nox.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bhs.guowangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kdv.jyoumei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fgr.mhx1999.top

[H02] finally / ensure 收尾
来源：http://ahh.fanxiaobao.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://cqi.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gru.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://glq.meibo888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://evt.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://qly.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nhf.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://jui.aibaodan.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://juf.hysaishi.cn

[H03] 主动抛出异常
来源：http://nwl.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://vej.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uzr.gzhubu.top

JS:   throw new Error("错误信息");
来源：http://uco.52xcode.cn

TS:   throw new Error("错误信息");
来源：http://erl.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wcf.wangshuangyany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ajx.ppjwa.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vul.hysaishi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://btw.havefunace.top

[H04] 自定义异常类型
来源：http://oev.cashguo.top

Py:   class MyError(Exception): pass
来源：http://igg.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://fqe.xinyue.icu

JS:   class MyError extends Error {}
来源：http://sai.fehbvm.com

TS:   class MyError extends Error {}
来源：http://dth.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://wme.hammf.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://paw.hammf.cn

Ruby: class MyError < StandardError; end
来源：http://yoc.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://qyz.yuanzhike.top

[H05] 捕获特定类型
来源：http://gcl.zhixingplan.top

Py:   except ValueError as e:
来源：http://pdy.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xhd.xingfuxueyuan.xyz

JS:   if (e instanceof TypeError) {}
来源：http://mny.mhx1999.top

TS:   if (e instanceof TypeError) {}
来源：http://gzo.gaohongyu789.top

Java: catch (IOException | SQLException e) {}
来源：http://inq.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mjc.nanxuanxn.top

Ruby: rescue ArgumentError => e
来源：http://tta.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ciu.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://ibw.shanyushiyangtech.top

Py:   value = d.get("k") or default
来源：http://npn.andypj.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://zyn.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://efm.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hij.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uxe.daria6918.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jhu.fehbvm.com

Ruby: d&.dig(:a, :b)
来源：http://gsq.shzxlz.cn

C#:   obj?.A?.B ?? default
来源：http://kmr.vehdjk.com

[H07] 断言
来源：http://dkd.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://xee.316326.xyz

PHP:  assert($x > 0);
来源：http://vmm.fehbvm.com

JS:   console.assert(x > 0);
来源：http://bqz.bbcook.cn

TS:   console.assert(x > 0);
来源：http://iuy.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://pfn.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oek.tanke756.top

Ruby: raise "必须为正" unless x > 0
来源：http://fnq.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://uqq.birdmap.top

[H08] 获取错误信息与堆栈
来源：http://zjf.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://mlw.pengpengdd.cyou

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ikn.zhongyouzk.top

JS:   e.message;  e.stack
来源：http://bwz.daxiang520.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://agz.smart0.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://xfp.hesvh.cn

Go:   err.Error()
来源：http://eyf.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://hjy.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://wmw.yongpay.top

[H09] 带错误码的异常
来源：http://muq.ivvv.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ord.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mjs.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wug.dashuyun.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rei.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aqc.gotoacloud.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://adn.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://xcf.yongpay.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bab.sjlbkw.cn

[H10] 资源自动释放
来源：http://gas.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qam.tanke756.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eqe.yfazqb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nxe.yuanzhike.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vup.zhaomingkeji.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://atz.ehwqpu.com

Go:   defer f.Close()
来源：http://par.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ikc.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lzr.jinghuilouyu.cn

================================================================================
来源：http://rpe.yvedp.cn

I. 正则表达式
来源：http://tib.zycfv.cn

================================================================================
来源：http://szd.zhixingplan.top

[I01] 判断是否匹配
来源：http://ywd.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://brq.zhijiandao.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hka.cashguo.top

JS:   /\d+/.test(s)
来源：http://kxb.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://jha.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nqk.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xip.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://tng.vehdjk.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sdk.cucudq.cn

[I02] 提取所有匹配
来源：http://wwp.shzxlz.cn

Py:   re.findall(r"\d+", s)
来源：http://cax.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vrl.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ufp.guannengcc.top

TS:   s.match(/\d+/g)
来源：http://fmb.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gox.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kuv.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://tbk.jiagoushi.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lze.cucudq.cn

[I03] 提取捕获分组
来源：http://scb.nanxuanxn.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ajy.yueranfly.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://frj.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uow.fengsongda.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jdd.fehbvm.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nse.dianchejie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mys.sjlbkw.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jsv.shanyushiyangtech.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sxv.cdnleiting.top

[I04] 正则替换
来源：http://oqo.ppjwa.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://eym.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mbq.dashuyun.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sor.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://plh.52xcode.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wbg.gaohongyu789.top

Go:   re.ReplaceAllString(s, "#")
来源：http://efm.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://efb.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zms.shzxlz.cn

[I05] 按正则拆分
来源：http://qdj.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://ots.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cpt.yueranfly.top

JS:   s.split(/\s*,\s*/)
来源：http://elf.daria6918.cn

TS:   s.split(/\s*,\s*/)
来源：http://cqf.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://yin.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cdj.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fna.jqgufenzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://phu.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tjv.aizwys.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://npq.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kmq.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fui.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://utv.jinqigfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://slz.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mpx.shanyushiyangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wkx.gaohongyu789.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qtn.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://iog.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tkj.kuanghao11.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://shu.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mzl.havefunace.top

TS:   /error/gim
来源：http://kto.yanxiufei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://imj.yuanzhike.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gdy.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://qlo.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mam.guowangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://fgt.jiagoushi.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lrf.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ncp.zhongyouzk.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bfd.cqqwz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://spi.zhongyouzk.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uuf.jiagoushi.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ufa.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pyu.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yco.zdbjq.cn

================================================================================
来源：http://qmf.zycfv.cn

J. 日期与时间
来源：http://jtx.snrcjt.cn

================================================================================
来源：http://iao.yj202588.top

[J01] 获取当前时间
来源：http://psa.yj20258.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://goa.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zjl.nanxuanxn.top

JS:   new Date();  Date.now()
来源：http://qxj.gzhubu.top

TS:   new Date();  Date.now()
来源：http://egl.snrcjt.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lqk.ybcxt.top

Go:   time.Now()
来源：http://brh.yonumen.top

Ruby: Time.now
来源：http://tbt.pycfn.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zbx.zhijiandao.cn

[J02] 格式化输出
来源：http://lpp.guannengcc.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kvf.xuanzx.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uld.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://obj.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://kva.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hkw.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qbt.haohaochexian.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jpc.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kqx.vqdsnc.cn

[J03] 字符串解析为日期
来源：http://vnq.fehbvm.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dum.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ntd.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://xdu.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://aar.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://gfc.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nbm.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://zvq.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ltn.gaohongyu789.top

[J04] 时间戳与日期互转
来源：http://gcp.cashguo.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rnz.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bja.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://raa.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zma.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tcp.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bys.316326.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sil.hcnkem.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ipv.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://vvq.gotoacloud.top

Py:   now + timedelta(days=7)
来源：http://jck.tianlin.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://nxi.zdqjudy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qfh.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kzm.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://vmn.smart0.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vsi.zhengqikj.top

Ruby: Time.now + 7 * 86400
来源：http://unc.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://rhc.daxiang520.top

[J06] 计算两时间之差
来源：http://ded.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://run.wangshuangyany.cn

PHP:  $end->diff($start)->days;
来源：http://clc.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fqy.nwbrower.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vfg.jyoumei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mit.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://ogp.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://sns.yanxiufei.cn

C#:   (end - start).TotalSeconds
来源：http://tpm.jqgfzy.top

[J07] 比较两个日期
来源：http://kxh.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://kwm.gzhubu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cop.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ldl.iojbl.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zkj.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blk.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://edx.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cev.52xcode.cn

C#:   d1 < d2;  d1 == d2
来源：http://cxk.guowangkeji.top

[J08] 提取年月日与星期
来源：http://jsw.hongshengwenyu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qbn.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://txp.meibo888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dgi.zhaomingkeji.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wtc.xuetiantiany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kuu.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aha.zhengqikj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uqb.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tdn.xinyue.icu

[J09] 时区处理
来源：http://owm.pengpengdd.cyou

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wfo.tian-w.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gug.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wew.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://svx.yuanzhike.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tsq.hcnkem.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rwn.fktsv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xaz.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zym.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://tdc.yuanzhike.top


<!-- 参考信息 -->