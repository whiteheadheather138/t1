代发 wailian999

Py:   isinstance(u, User)
来源：http://qrh.hammf.cn

PHP:  $u instanceof User
来源：http://xjt.chenzaomai.com

JS:   u instanceof User
来源：http://spi.yj20258888.top

TS:   u instanceof User
来源：http://zlr.ydjk.org.cn

Java: u instanceof User
来源：http://gzt.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ypd.yj20258888.top

Ruby: u.is_a?(User)
来源：http://clc.sjlbkw.cn

C#:   u is User
来源：http://rps.ivvv.top

[G14] 数据类 / record
来源：http://pxo.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dqi.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://yek.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bsg.zdqjudy.top

TS:   type User = { name: string; age: number };
来源：http://gll.yvedp.cn

Java: record User(String name, int age) {}
来源：http://gik.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://lmv.birdmap.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qqc.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://tbs.havefunace.top

[G15] 枚举
来源：http://efb.yj20258.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pyi.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://uor.feifeiyinyue.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uoh.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fst.fehbvm.com

Java: enum Color { RED, GREEN }
来源：http://qbv.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uje.haohaochexian.top

Ruby: Color = %i[red green].freeze
来源：http://voe.gaohongyu789.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://chf.fanxiaobao.xyz

[G16] 对象转数组 / 字典
来源：http://kux.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vuh.sweek.top

PHP:  get_object_vars($obj);
来源：http://lot.hnqzz.top

JS:   Object.entries(obj)
来源：http://dcx.vehdjk.com

TS:   Object.entries(obj)
来源：http://isc.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mcx.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zcy.cheryme.top

Ruby: obj.instance_variables
来源：http://mro.jqgufenzy.top

C#:   // 用反射或 System.Text.Json
来源：http://icp.hcnkem.com

================================================================================
来源：http://zol.pengpengdd.cyou

H. 异常与错误处理
来源：http://hfl.zhengqikj.top

================================================================================
来源：http://oih.vqdsnc.cn

[H01] try / catch 基础
来源：http://wii.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rch.cdnleiting.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://veh.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vfs.zhengqikj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oad.redwolf501.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wkg.zdbjq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fhi.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ben.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tzo.hesvh.cn

[H02] finally / ensure 收尾
来源：http://kmq.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://qyr.hesvh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dhx.zdqjudy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vdn.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vzi.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://xnq.hongshengwenyu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bav.xuanzx.com

Ruby: begin; f; ensure; cleanup; end
来源：http://iwe.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cjh.jlsjyb.cn

[H03] 主动抛出异常
来源：http://wir.tanke756.top

Py:   raise ValueError("错误信息")
来源：http://uux.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mai.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://eyq.sweek.top

TS:   throw new Error("错误信息");
来源：http://uva.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vsk.havefunace.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ybk.zycfv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sod.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yxe.redwolf501.top

[H04] 自定义异常类型
来源：http://lsb.yj20258.top

Py:   class MyError(Exception): pass
来源：http://ysf.ybcxt.top

PHP:  class MyError extends RuntimeException {}
来源：http://cgx.guannengcc.top

JS:   class MyError extends Error {}
来源：http://prx.gzhubu.top

TS:   class MyError extends Error {}
来源：http://gdh.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://blr.daria6918.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://osa.xuanzx.com

Ruby: class MyError < StandardError; end
来源：http://dyi.yuxming.cn

C#:   class MyException : Exception {}
来源：http://owb.tianlin.xyz

[H05] 捕获特定类型
来源：http://fuj.mhx1999.top

Py:   except ValueError as e:
来源：http://hid.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mqd.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://pbd.gzhubu.top

TS:   if (e instanceof TypeError) {}
来源：http://odx.gaohongyu789.top

Java: catch (IOException | SQLException e) {}
来源：http://pnt.hywenlv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zon.tanke756.top

Ruby: rescue ArgumentError => e
来源：http://xof.zhijiandao.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tvh.guannengcc.top

[H06] 可选值 / 空值安全访问
来源：http://hdd.yueranfly.top

Py:   value = d.get("k") or default
来源：http://hzk.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fvk.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://wcb.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kjy.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sbv.shanyushiyangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zwm.jlsjyb.cn

Ruby: d&.dig(:a, :b)
来源：http://jwp.guowangkeji.top

C#:   obj?.A?.B ?? default
来源：http://mft.yj20258.top

[H07] 断言
来源：http://btu.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://imu.yuxming.cn

PHP:  assert($x > 0);
来源：http://tyb.chenlongwang.top

JS:   console.assert(x > 0);
来源：http://sap.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://orq.fktsv.cn

Java: assert x > 0 : "必须为正";
来源：http://apg.chenjidiqi.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mku.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://mcu.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://ija.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://lni.dianchejie.cn

Py:   str(e);  traceback.format_exc()
来源：http://sjc.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://onw.yj202588.top

JS:   e.message;  e.stack
来源：http://aci.xingfuxueyuan.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://loy.yanxiufei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wfk.wangdashe.top

Go:   err.Error()
来源：http://hpf.gaohongyu789.top

Ruby: e.message;  e.backtrace
来源：http://vvg.yueranfly.top

C#:   e.Message;  e.StackTrace
来源：http://iuk.aizwys.cn

[H09] 带错误码的异常
来源：http://vof.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jxq.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://aec.nanxuanxn.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ini.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rnj.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uuw.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://emh.xinyue.icu

Ruby: raise MyError.new("fail", 500)
来源：http://ufs.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qvh.smart0.xyz

[H10] 资源自动释放
来源：http://kul.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ngc.sxryk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xnl.zhiwuduotai.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pou.yuxming.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tdx.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://beu.zycfv.cn

Go:   defer f.Close()
来源：http://tbb.zhijiandao.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://phm.hywenlv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wrc.shanyushiyangtech.top

================================================================================
来源：http://uff.0kj1m.cn

I. 正则表达式
来源：http://wiy.xinyue.icu

================================================================================
来源：http://mir.hywenlv.cn

[I01] 判断是否匹配
来源：http://qek.meibo888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nnr.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://yzm.havefunace.top

JS:   /\d+/.test(s)
来源：http://yuz.hywenlv.cn

TS:   /\d+/.test(s)
来源：http://vdw.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://otv.yueranfly.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://irz.gzhubu.top

Ruby: s.match?(/\d+/)
来源：http://pfx.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cie.hammf.cn

[I02] 提取所有匹配
来源：http://mpp.52xcode.cn

Py:   re.findall(r"\d+", s)
来源：http://ynb.jlsjyb.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fbz.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bmd.bjfxy.top

TS:   s.match(/\d+/g)
来源：http://trd.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bzu.hammf.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yke.zhaomingkeji.xyz

Ruby: s.scan(/\d+/)
来源：http://ssk.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tsg.zhongyouzk.top

[I03] 提取捕获分组
来源：http://lqc.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wgv.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oym.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://swr.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://phz.zhongyouzk.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yvv.yfazqb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hkg.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bvi.ehwqpu.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bov.iojbl.cn

[I04] 正则替换
来源：http://bfr.chenjidiqi.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://jpd.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xxf.yuxming.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zcp.nanxinkj.top

TS:   s.replace(/\d+/g, "#")
来源：http://soz.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fsr.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oeo.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wxq.chenlongwang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oqh.yongpay.top

[I05] 按正则拆分
来源：http://ymv.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://raf.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gds.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://dhw.nanxuanxn.top

TS:   s.split(/\s*,\s*/)
来源：http://rjo.shzxlz.cn

Java: s.split("\\s*,\\s*")
来源：http://bst.hywenlv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gsc.zhoulong.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://xhs.jqgufenzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jyo.fehbvm.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mgz.yonumen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ffu.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lbm.sysykeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qxg.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mim.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rhk.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zgg.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mjr.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uid.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://edg.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yxk.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hzc.nanxuanxn.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ubw.tianlin.xyz

TS:   /error/gim
来源：http://yie.shanyushiyangtech.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kmr.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://seg.pengpengdd.cyou

Ruby: s.scan(/error/i)
来源：http://ogq.smart0.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bac.bbcook.cn

[I08] 贪婪与非贪婪匹配
来源：http://kdl.snrcjt.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kuu.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pls.ybcxt.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pdi.jyoumei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oaz.bbcook.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://clh.aibaodan.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nee.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ukc.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xbx.fengsongda.top

================================================================================
来源：http://ihu.hesvh.cn

J. 日期与时间
来源：http://dqu.jianghu66.top

================================================================================
来源：http://qzx.iojbl.cn

[J01] 获取当前时间
来源：http://tmz.gotoacloud.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xii.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wuc.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://fjr.mhx1999.top

TS:   new Date();  Date.now()
来源：http://nqk.cucudq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hrh.zhiwuduotai.top

Go:   time.Now()
来源：http://hld.zhongyouzk.top

Ruby: Time.now
来源：http://cfv.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kqn.tanke756.top

[J02] 格式化输出
来源：http://zbq.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dep.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yvq.gotoacloud.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kpw.gogol.net.cn

TS:   d.toISOString()
来源：http://ekt.uphjek.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hoq.mhx1999.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dco.jinqigfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gxu.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xue.sweek.top

[J03] 字符串解析为日期
来源：http://cmk.hfpthk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xah.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pmk.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://rfc.gotoacloud.top

TS:   new Date("2024-01-02")
来源：http://rjz.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://aol.haohaochexian.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hwp.smart0.xyz

Ruby: Date.parse("2024-01-02")
来源：http://wzg.cqqwz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ttu.shuidangran.top

[J04] 时间戳与日期互转
来源：http://rcy.nanxuanxn.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://izj.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uyp.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://brp.guannengcc.top

TS:   Math.floor(Date.now() / 1000)
来源：http://avp.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fbo.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ppd.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://onb.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xpt.mhx1999.top

[J05] 时间加减（加 7 天）
来源：http://upn.sxryk.cn

Py:   now + timedelta(days=7)
来源：http://lgr.zhaomingkeji.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://hxx.sweek.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xjf.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://phx.jinyuanbaomall.cn

Java: LocalDate.now().plusDays(7)
来源：http://umv.jqgfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://omc.feifeiyinyue.top

Ruby: Time.now + 7 * 86400
来源：http://ovp.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://oab.sxryk.cn

[J06] 计算两时间之差
来源：http://rzm.guannengcc.top

Py:   (end - start).total_seconds()
来源：http://ete.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://bza.zhixingplan.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oan.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kzw.yangfankeji.com

Java: Duration.between(start, end).toSeconds()
来源：http://bsa.snrcjt.cn

Go:   end.Sub(start).Hours()
来源：http://vgr.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://ijf.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://qqb.fehbvm.com

[J07] 比较两个日期
来源：http://mjx.cqqwz.cn

Py:   d1 < d2;  d1 == d2
来源：http://iev.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fyf.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://rhj.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rhw.snrcjt.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oew.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rnt.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://ypc.hongshengwenyu.top

C#:   d1 < d2;  d1 == d2
来源：http://fqj.sweek.top

[J08] 提取年月日与星期
来源：http://qgx.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jfu.nanxinkj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nle.haohaochexian.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jfl.pycfn.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ssf.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jjk.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aji.nanxuanxn.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gwc.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ryx.xinyue.icu

[J09] 时区处理
来源：http://baj.shuidangran.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tur.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qcv.yongpay.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kpj.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nhs.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iok.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ufz.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xdo.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hnx.xziqi.cn

[J10] 取今天 / 本月第一天
来源：http://kon.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://acn.zycfv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sae.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xbt.jiagoushi.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uzd.zhijiandao.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cax.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ruq.tanke756.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ijo.zhijiandao.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ubi.hysaishi.cn

================================================================================
来源：http://hvu.yuxming.cn

K. JSON 与序列化
来源：http://wby.tarul.cn

================================================================================
来源：http://mvh.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://dnp.ivvv.top


<!-- 参考信息 -->