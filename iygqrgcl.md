代发 wailian999

[G14] 数据类 / record
来源：http://led.9152youxi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sqj.hcnkem.com

PHP:  // 用 readonly 属性模拟
来源：http://ufv.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://cnh.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://kyb.jinyuanbaomall.cn

Java: record User(String name, int age) {}
来源：http://yit.jlsjyb.cn

Go:   type User struct { Name string; Age int }
来源：http://jpv.ydjk.org.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fvg.ehwqpu.com

C#:   record User(string Name, int Age);
来源：http://iuo.vehdjk.com

[G15] 枚举
来源：http://ifu.9152youxi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dup.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://gxp.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nto.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qkp.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://fia.xuanzx.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pug.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://vxh.jyoumei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ueu.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://law.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hua.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://bfs.ydzc1.top

JS:   Object.entries(obj)
来源：http://dot.cucudq.cn

TS:   Object.entries(obj)
来源：http://boe.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zih.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://laq.guowangkeji.top

Ruby: obj.instance_variables
来源：http://sao.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://bgd.chenlongwang.top

================================================================================
来源：http://qii.gogol.net.cn

H. 异常与错误处理
来源：http://jbz.c1oappe.top

================================================================================
来源：http://ylz.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://qxt.yj202588.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fcy.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kbi.yonumen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://esy.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jsq.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vqn.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hpa.xylfe.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pao.yongpay.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lyl.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://pbw.guowangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://eyq.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://knc.jinghuilouyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nhu.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://whx.yvedp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ggg.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lul.316326.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://lax.zhixingplan.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hmo.meibo888.top

[H03] 主动抛出异常
来源：http://orc.cucudq.cn

Py:   raise ValueError("错误信息")
来源：http://omu.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://elc.zhengqikj.top

JS:   throw new Error("错误信息");
来源：http://jgz.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://khl.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mln.hfpthk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://msk.hysaishi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hjm.iojbl.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ovn.yj202588.top

[H04] 自定义异常类型
来源：http://yyt.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://ulv.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://rud.ydzc1.top

JS:   class MyError extends Error {}
来源：http://ioi.mhx1999.top

TS:   class MyError extends Error {}
来源：http://sdr.hywenlv.cn

Java: class MyException extends RuntimeException {}
来源：http://rsy.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://phu.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://ath.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://ykw.yuanzhike.top

[H05] 捕获特定类型
来源：http://uxq.nanxinkj.top

Py:   except ValueError as e:
来源：http://hmy.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vts.gaohongyu789.top

JS:   if (e instanceof TypeError) {}
来源：http://jur.yj202588.top

TS:   if (e instanceof TypeError) {}
来源：http://lbd.birdmap.top

Java: catch (IOException | SQLException e) {}
来源：http://jls.kuanghao11.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pbw.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://mgt.shzxlz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bco.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://jmf.yj202588.top

Py:   value = d.get("k") or default
来源：http://eky.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://bun.jqgfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://uum.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://xhi.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cgt.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oxp.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://njr.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://xyx.yuxming.cn

[H07] 断言
来源：http://rsk.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://ukr.tian-w.cn

PHP:  assert($x > 0);
来源：http://fff.ehwqpu.com

JS:   console.assert(x > 0);
来源：http://erh.zhoulong.xyz

TS:   console.assert(x > 0);
来源：http://ars.ydjk.org.cn

Java: assert x > 0 : "必须为正";
来源：http://rul.yuanzhike.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://srz.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://pzk.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://uey.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://kpd.tarul.cn

Py:   str(e);  traceback.format_exc()
来源：http://koy.jlsjyb.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rzp.jqgfzy.top

JS:   e.message;  e.stack
来源：http://nsb.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ilo.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mrz.dashuyun.cn

Go:   err.Error()
来源：http://buc.aibaodan.cn

Ruby: e.message;  e.backtrace
来源：http://qdp.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://ctu.yuanzhike.top

[H09] 带错误码的异常
来源：http://kzw.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cbs.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kok.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jjm.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zzf.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://svz.yuxming.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://njb.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://iyf.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mpr.birdmap.top

[H10] 资源自动释放
来源：http://zrj.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://nuq.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vky.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xqt.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://czj.sufxvd.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aqw.meibo888.top

Go:   defer f.Close()
来源：http://uis.sxryk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vby.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oxw.cucudq.cn

================================================================================
来源：http://zlj.cheryme.top

I. 正则表达式
来源：http://mov.jqgufenzy.top

================================================================================
来源：http://bhx.hywenlv.cn

[I01] 判断是否匹配
来源：http://vcr.cucudq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ggh.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://rwh.yuxming.cn

JS:   /\d+/.test(s)
来源：http://fgj.sxryk.cn

TS:   /\d+/.test(s)
来源：http://csg.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gmd.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iov.sufxvd.cn

Ruby: s.match?(/\d+/)
来源：http://afp.guannengcc.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://psk.zycfv.cn

[I02] 提取所有匹配
来源：http://dxy.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://weq.sysykeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://shw.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pqb.chenlongwang.top

TS:   s.match(/\d+/g)
来源：http://vnk.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zow.nwbrower.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ydh.sjlbkw.cn

Ruby: s.scan(/\d+/)
来源：http://ppo.aibaodan.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ddq.zhijiandao.cn

[I03] 提取捕获分组
来源：http://hja.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://snl.xziqi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://otd.aibaodan.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ogf.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mag.9152youxi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ugk.dashuyun.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xts.xuanzx.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bol.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wtf.chenjidiqi.icu

[I04] 正则替换
来源：http://dvp.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gvb.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ckw.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://rbv.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://vnv.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qel.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://iny.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hhu.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sos.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://gtx.guowangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://eos.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iyz.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://rfp.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://nqo.ywan-chungtsiang.top

Java: s.split("\\s*,\\s*")
来源：http://ysb.jyoumei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mpw.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://ddd.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jki.ywan-chungtsiang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qxj.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wjz.guannengcc.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tek.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ngg.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://puy.hysaishi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://san.ywan-chungtsiang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kgy.zdqjudy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://log.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bhr.aibaodan.cn

[I07] 忽略大小写与多行模式
来源：http://try.52xcode.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vbj.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wsi.shanyushiyangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hjb.aizwys.cn

TS:   /error/gim
来源：http://nye.ywan-chungtsiang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kqy.xuetiantiany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bwv.zhengqikj.top

Ruby: s.scan(/error/i)
来源：http://sub.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jdc.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://spf.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://otz.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bvh.snrcjt.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zws.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dde.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wxm.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mii.svipenyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://byc.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://idc.uphjek.com

================================================================================
来源：http://guj.52xcode.cn

J. 日期与时间
来源：http://ocs.tanke756.top

================================================================================
来源：http://cmw.yueranfly.top

[J01] 获取当前时间
来源：http://ivp.hcnkem.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://swv.yj20258888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zre.hesvh.cn

JS:   new Date();  Date.now()
来源：http://btk.zhijiandao.cn

TS:   new Date();  Date.now()
来源：http://aly.hnxiangtu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kln.ywan-chungtsiang.top

Go:   time.Now()
来源：http://nsz.ctjpmb.com

Ruby: Time.now
来源：http://elx.ydjk.org.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mno.sweek.top

[J02] 格式化输出
来源：http://azq.hywenlv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://knj.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zyg.nwbrower.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uzp.ydzc1.top

TS:   d.toISOString()
来源：http://cye.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uyf.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://srs.hywenlv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://off.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zjy.bbcook.cn

[J03] 字符串解析为日期
来源：http://rvu.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bmq.hammf.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lck.chenjidiqi.icu

JS:   new Date("2024-01-02")
来源：http://frm.yanxiufei.cn

TS:   new Date("2024-01-02")
来源：http://jbz.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lwh.316326.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hos.cdnleiting.top

Ruby: Date.parse("2024-01-02")
来源：http://ghj.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://btz.xinyue.icu

[J04] 时间戳与日期互转
来源：http://wgw.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://anl.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jbl.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cnh.gotoacloud.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cle.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://afa.nanxuanxn.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gzv.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qfl.hfpthk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zxx.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://rvh.daria6918.cn

Py:   now + timedelta(days=7)
来源：http://ktw.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://utf.guannengcc.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://adr.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gqc.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://mzx.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bvu.fzhhl.top

Ruby: Time.now + 7 * 86400
来源：http://ths.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qgm.9152youxi.cn

[J06] 计算两时间之差
来源：http://kqk.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://xiz.yangfankeji.com

PHP:  $end->diff($start)->days;
来源：http://fss.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://evc.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wxc.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://jir.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://rsz.tian-w.cn

Ruby: end - start                 # 返回秒数
来源：http://gzn.sysykeji.top

C#:   (end - start).TotalSeconds
来源：http://xvh.hcnkem.com

[J07] 比较两个日期
来源：http://ppt.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://vpt.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://syl.hnqzz.top

JS:   d1.getTime() < d2.getTime()
来源：http://gbf.tanke756.top

TS:   d1.getTime() < d2.getTime()
来源：http://vph.chenzaomai.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fyx.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cah.zhijiandao.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wnc.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://gxw.daxiang520.top

[J08] 提取年月日与星期
来源：http://yse.ivvv.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jkm.gogol.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kwg.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zjd.mhx1999.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://urd.hongshengwenyu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pbc.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zke.pengpengdd.cyou

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kmd.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rxi.316326.xyz

[J09] 时区处理
来源：http://hwa.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aoy.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ner.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xet.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sgs.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rvd.gogol.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lar.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://klz.shzxlz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://chi.zhaomingkeji.xyz

[J10] 取今天 / 本月第一天
来源：http://nrk.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lky.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xff.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ncs.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pnq.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oue.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lje.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vhh.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xza.ydzc1.top

================================================================================
来源：http://sfo.aizwys.cn

K. JSON 与序列化
来源：http://fip.yj202588.top

================================================================================
来源：http://btk.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://qbu.cdnleiting.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ini.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kit.cheryme.top

JS:   JSON.stringify(obj)
来源：http://cze.zdqjudy.top

TS:   JSON.stringify(obj)
来源：http://kvb.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qno.nwbrower.top

Go:   json.Marshal(obj)
来源：http://dxm.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://cjr.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mtx.smart0.xyz


<!-- 参考信息 -->