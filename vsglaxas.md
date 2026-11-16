代发 wailian999

[G14] 数据类 / record
来源：http://hge.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tsq.aibaodan.cn

PHP:  // 用 readonly 属性模拟
来源：http://ovk.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://abd.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://zds.fengsongda.top

Java: record User(String name, int age) {}
来源：http://our.zhiwuduotai.top

Go:   type User struct { Name string; Age int }
来源：http://rnu.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iod.ywan-chungtsiang.top

C#:   record User(string Name, int Age);
来源：http://ukv.hongshengwenyu.top

[G15] 枚举
来源：http://gmh.ybcxt.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bcr.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rap.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fae.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uzb.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://urp.vehdjk.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nkf.tarul.cn

Ruby: Color = %i[red green].freeze
来源：http://gej.quarkkingdee.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rcm.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://otb.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uxk.sufxvd.cn

PHP:  get_object_vars($obj);
来源：http://qxw.daria6918.cn

JS:   Object.entries(obj)
来源：http://duw.zycfv.cn

TS:   Object.entries(obj)
来源：http://zdo.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yct.gaohongyu789.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ayu.hnqzz.top

Ruby: obj.instance_variables
来源：http://kao.tarul.cn

C#:   // 用反射或 System.Text.Json
来源：http://dwb.hysaishi.cn

================================================================================
来源：http://ezk.wangdashe.top

H. 异常与错误处理
来源：http://irn.gogol.net.cn

================================================================================
来源：http://bvt.fktsv.cn

[H01] try / catch 基础
来源：http://nbn.shzxlz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xoo.9152youxi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fia.andypj.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yhn.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bld.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jnh.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uvg.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rme.ivvv.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://igw.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://ybd.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://snb.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xrk.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pzs.vehdjk.com

TS:   try { f(); } finally { cleanup(); }
来源：http://uep.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://sks.bjfxy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ytz.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rxo.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://edz.52xcode.cn

[H03] 主动抛出异常
来源：http://sxu.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://iro.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ged.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://htx.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://whq.yonumen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jvv.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kyh.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://lke.xinyue.icu

C#:   throw new ArgumentException("错误信息");
来源：http://one.zhengqikj.top

[H04] 自定义异常类型
来源：http://vid.gogol.net.cn

Py:   class MyError(Exception): pass
来源：http://pul.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://ext.meibo888.top

JS:   class MyError extends Error {}
来源：http://whj.ivvv.top

TS:   class MyError extends Error {}
来源：http://tmm.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://wex.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lph.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://arj.cdnleiting.top

C#:   class MyException : Exception {}
来源：http://omi.svipenyu.cn

[H05] 捕获特定类型
来源：http://gpz.zdqjudy.top

Py:   except ValueError as e:
来源：http://uth.zhijiandao.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aiv.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://ihe.shangyingyoupin.top

TS:   if (e instanceof TypeError) {}
来源：http://xaq.haohaochexian.top

Java: catch (IOException | SQLException e) {}
来源：http://tdl.chenjidiqi.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://avm.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://uwu.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wpi.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://ypo.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://fbh.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://qog.zhiwuduotai.top

JS:   obj?.a?.b;  d ?? default
来源：http://ptr.9152youxi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pcy.jinyuanbaomall.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zfy.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jxm.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://itr.smart0.xyz

C#:   obj?.A?.B ?? default
来源：http://rik.cucudq.cn

[H07] 断言
来源：http://had.andypj.xyz

Py:   assert x > 0, "必须为正"
来源：http://cid.andypj.xyz

PHP:  assert($x > 0);
来源：http://ksa.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://xkk.zdbjq.cn

TS:   console.assert(x > 0);
来源：http://xuw.fktsv.cn

Java: assert x > 0 : "必须为正";
来源：http://tob.hammf.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wso.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wpn.fehbvm.com

C#:   Debug.Assert(x > 0);
来源：http://vba.jianghu66.top

[H08] 获取错误信息与堆栈
来源：http://etz.shanyushiyangtech.top

Py:   str(e);  traceback.format_exc()
来源：http://mes.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iso.jinghuilouyu.cn

JS:   e.message;  e.stack
来源：http://cbk.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://djo.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://iwh.sysykeji.top

Go:   err.Error()
来源：http://obo.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://vop.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://ugb.zhijiandao.cn

[H09] 带错误码的异常
来源：http://hzh.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jho.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ygn.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qtf.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rpv.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kvp.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dbd.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://gaq.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uex.zhoulong.xyz

[H10] 资源自动释放
来源：http://rdu.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xux.ctjpmb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://roo.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eag.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ubj.xingfuxueyuan.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lsd.sweek.top

Go:   defer f.Close()
来源：http://czm.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qtn.yvedp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mll.xziqi.cn

================================================================================
来源：http://lva.sufxvd.cn

I. 正则表达式
来源：http://bes.vehdjk.com

================================================================================
来源：http://lwe.hongshengwenyu.top

[I01] 判断是否匹配
来源：http://dkr.svipenyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mnr.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nif.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://jha.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://koa.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lfn.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jtn.nanxuanxn.top

Ruby: s.match?(/\d+/)
来源：http://prw.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hug.daria6918.cn

[I02] 提取所有匹配
来源：http://xns.svipenyu.cn

Py:   re.findall(r"\d+", s)
来源：http://hrs.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oyz.zdqjudy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ixo.xuanzx.com

TS:   s.match(/\d+/g)
来源：http://tix.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jvs.tanke756.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wnk.feifeiyinyue.top

Ruby: s.scan(/\d+/)
来源：http://tka.yanxiufei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zjl.yj20258.top

[I03] 提取捕获分组
来源：http://wdy.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ilc.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rlo.ydzc1.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gmv.uphjek.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mbj.zycfv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xjr.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ohz.gogol.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lgq.zhixingplan.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nce.wangdashe.top

[I04] 正则替换
来源：http://nho.yvedp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://voz.daxiang520.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lam.nwbrower.top

JS:   s.replace(/\d+/g, "#")
来源：http://vqb.fehbvm.com

TS:   s.replace(/\d+/g, "#")
来源：http://zxj.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://vjs.mhx1999.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mny.yfazqb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://xlt.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nfm.gogol.net.cn

[I05] 按正则拆分
来源：http://uko.wangshuangyany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gtm.wangdashe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gqg.yanxiufei.cn

JS:   s.split(/\s*,\s*/)
来源：http://lya.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://snf.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://ytx.kuanghao11.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qiu.dianchejie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://reo.dianchejie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hfb.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fwa.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lta.ybcxt.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sax.zhixingplan.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iex.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tul.jinqigufen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gay.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cec.yongpay.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://raq.ywan-chungtsiang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qlw.vqdsnc.cn

[I07] 忽略大小写与多行模式
来源：http://bnl.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tai.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ryz.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pet.yueranfly.top

TS:   /error/gim
来源：http://cwa.hnqzz.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fcs.birdmap.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://itt.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://omy.zhoulong.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uhu.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://nee.jinqigufen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ose.shanyushiyangtech.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gcu.vqdsnc.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fdo.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bjw.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tir.redwolf501.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://olq.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kwf.hnxiangtu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zdm.pengpengdd.cyou

================================================================================
来源：http://cmq.chenlongwang.top

J. 日期与时间
来源：http://mrg.sweek.top

================================================================================
来源：http://tli.zdbjq.cn

[J01] 获取当前时间
来源：http://dtr.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bwi.jinghuilouyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vgu.yangfankeji.com

JS:   new Date();  Date.now()
来源：http://syu.yj20258888.top

TS:   new Date();  Date.now()
来源：http://qnr.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xiq.tarul.cn

Go:   time.Now()
来源：http://szv.yvedp.cn

Ruby: Time.now
来源：http://apn.uphjek.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tyc.ehwqpu.com

[J02] 格式化输出
来源：http://umq.xingfuxueyuan.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qtx.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hck.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://obz.jiagoushi.top

TS:   d.toISOString()
来源：http://poo.nanxuanxn.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dka.sxryk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nrf.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pqo.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bqm.yj20258888.top

[J03] 字符串解析为日期
来源：http://jbi.aibaodan.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hjk.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oqw.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://sto.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://fli.zhixingplan.top

Java: LocalDate.parse("2024-01-02")
来源：http://rdf.guannengcc.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ysn.nanxuanxn.top

Ruby: Date.parse("2024-01-02")
来源：http://agp.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zts.ppjwa.cn

[J04] 时间戳与日期互转
来源：http://yup.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tvi.sjlbkw.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yzx.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lxn.zhijiandao.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://myf.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://isy.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uyh.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dea.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://thp.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://ove.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://eyn.ppjwa.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ezx.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wsi.cdnleiting.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://isq.tian-w.cn

Java: LocalDate.now().plusDays(7)
来源：http://ssj.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mps.zdbjq.cn

Ruby: Time.now + 7 * 86400
来源：http://cvn.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://zpu.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://nlk.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://fir.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://ngu.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hdk.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://spt.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://bcd.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://byg.chenjidiqi.icu

Ruby: end - start                 # 返回秒数
来源：http://dqw.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://ipm.andypj.xyz

[J07] 比较两个日期
来源：http://crm.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://cpq.zhengqikj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jjy.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://tbr.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://anv.316326.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://evp.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ajm.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://mhj.yfazqb.com

C#:   d1 < d2;  d1 == d2
来源：http://xug.wangdashe.top

[J08] 提取年月日与星期
来源：http://fow.jqgfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://neb.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hhg.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fvz.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xpe.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mpm.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cbc.sufxvd.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zkc.yj20258.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gmo.yanxiufei.cn

[J09] 时区处理
来源：http://geo.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bwf.yonumen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ymd.fktsv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lpk.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ela.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://whd.zdqjudy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mhl.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://viw.sjlbkw.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jfx.chenlongwang.top

[J10] 取今天 / 本月第一天
来源：http://hly.jqgfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://toa.fengsongda.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ntt.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wnv.sufxvd.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qsr.yj20258888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://abe.yanxiufei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ufw.cqqwz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lld.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xqm.yuxming.cn

================================================================================
来源：http://rag.xinyue.icu

K. JSON 与序列化
来源：http://oym.fengsongda.top

================================================================================
来源：http://ire.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://zcw.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://edj.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nne.zhoulong.xyz

JS:   JSON.stringify(obj)
来源：http://cgl.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://xyb.52xcode.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zod.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://rij.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://pic.dashuyun.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mri.fehbvm.com


<!-- 参考信息 -->