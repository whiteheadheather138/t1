代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://acw.yj202588.top

Java: record User(String name, int age) {}
来源：http://smd.jianghu66.top

Go:   type User struct { Name string; Age int }
来源：http://oqv.cashguo.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jyv.yj202588.top

C#:   record User(string Name, int Age);
来源：http://gar.tianlin.xyz

[G15] 枚举
来源：http://hxi.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nac.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vam.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://seq.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ixb.shzxlz.cn

Java: enum Color { RED, GREEN }
来源：http://fvi.tanke756.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mtr.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://fho.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eoa.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://nkv.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gab.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://wld.yj202588.top

JS:   Object.entries(obj)
来源：http://xes.wangshuangyany.cn

TS:   Object.entries(obj)
来源：http://uik.aibaodan.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kbf.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vix.shzxlz.cn

Ruby: obj.instance_variables
来源：http://nxq.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://hmd.cucudq.cn

================================================================================
来源：http://eyg.xylfe.cn

H. 异常与错误处理
来源：http://jdr.yj202588.top

================================================================================
来源：http://ejq.vehdjk.com

[H01] try / catch 基础
来源：http://uvp.nwbrower.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vxq.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gke.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tgi.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://osq.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hqc.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jku.xuetiantiany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lub.mhx1999.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://quy.feifeiyinyue.top

[H02] finally / ensure 收尾
来源：http://jfv.guannengcc.top

Py:   try: f()⏎finally: cleanup()
来源：http://juo.iojbl.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cot.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ufm.birdmap.top

TS:   try { f(); } finally { cleanup(); }
来源：http://iys.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cow.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://slx.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jkl.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://tqc.zhijiandao.cn

[H03] 主动抛出异常
来源：http://olu.0kj1m.cn

Py:   raise ValueError("错误信息")
来源：http://fau.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ehl.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://hdf.pengpengdd.cyou

TS:   throw new Error("错误信息");
来源：http://pci.0kj1m.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rpw.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fnl.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vzj.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://hru.vqdsnc.cn

[H04] 自定义异常类型
来源：http://xbl.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://qgs.tianlin.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://npk.vqdsnc.cn

JS:   class MyError extends Error {}
来源：http://icz.meibo888.top

TS:   class MyError extends Error {}
来源：http://hyb.jinyuanbaomall.cn

Java: class MyException extends RuntimeException {}
来源：http://wwq.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lvf.hnqzz.top

Ruby: class MyError < StandardError; end
来源：http://zhs.bbcook.cn

C#:   class MyException : Exception {}
来源：http://uyy.mhx1999.top

[H05] 捕获特定类型
来源：http://tip.gotoacloud.top

Py:   except ValueError as e:
来源：http://kxr.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://trk.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://oml.xuetiantiany.cn

TS:   if (e instanceof TypeError) {}
来源：http://aoj.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://pgk.yuxming.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zul.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://ryr.zhongyouzk.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rvo.haohaochexian.top

[H06] 可选值 / 空值安全访问
来源：http://jkz.wangdashe.top

Py:   value = d.get("k") or default
来源：http://lsz.tianlin.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://dyi.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ykh.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wcf.hfpthk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rbe.smart0.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://uyh.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://bcj.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://yqh.shzxlz.cn

[H07] 断言
来源：http://cdh.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://fvl.0kj1m.cn

PHP:  assert($x > 0);
来源：http://exw.tian-w.cn

JS:   console.assert(x > 0);
来源：http://swm.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://wvn.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://crb.jinyuanbaomall.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ghk.jlsjyb.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hwh.cqqwz.cn

C#:   Debug.Assert(x > 0);
来源：http://msk.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://fjp.nwbrower.top

Py:   str(e);  traceback.format_exc()
来源：http://fux.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ajq.birdmap.top

JS:   e.message;  e.stack
来源：http://vpy.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uzm.sweek.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uem.nanxinkj.top

Go:   err.Error()
来源：http://nfl.jlsjyb.cn

Ruby: e.message;  e.backtrace
来源：http://hyp.daria6918.cn

C#:   e.Message;  e.StackTrace
来源：http://kwg.c1oappe.top

[H09] 带错误码的异常
来源：http://twf.xuanzx.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jhb.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vhc.gzhubu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bwy.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zam.daria6918.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lzz.wangdashe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nhl.hcnkem.com

Ruby: raise MyError.new("fail", 500)
来源：http://cjj.cheryme.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zsp.uphjek.com

[H10] 资源自动释放
来源：http://xwr.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zhe.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zgt.jyoumei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mpd.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://psi.gotoacloud.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xsq.zycfv.cn

Go:   defer f.Close()
来源：http://xpo.yongpay.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uwf.wangdashe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uom.zhaomingkeji.xyz

================================================================================
来源：http://sgu.xingfuxueyuan.xyz

I. 正则表达式
来源：http://gwz.guowangkeji.top

================================================================================
来源：http://jhk.tarul.cn

[I01] 判断是否匹配
来源：http://vuz.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ycu.tanke756.top

PHP:  preg_match('/\d+/', $s);
来源：http://sxg.snrcjt.cn

JS:   /\d+/.test(s)
来源：http://ufn.zhengqikj.top

TS:   /\d+/.test(s)
来源：http://nms.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://frg.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uqg.smart0.xyz

Ruby: s.match?(/\d+/)
来源：http://ppl.jyoumei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bih.c1oappe.top

[I02] 提取所有匹配
来源：http://wzv.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://hgi.nwbrower.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lkw.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nth.hywenlv.cn

TS:   s.match(/\d+/g)
来源：http://tae.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rpm.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zcw.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://ndp.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://twt.dianchejie.cn

[I03] 提取捕获分组
来源：http://sqq.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://knq.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bio.aibaodan.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qvr.chenlongwang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gej.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ycy.zhengqikj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://car.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vrs.hnxiangtu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://msx.ehwqpu.com

[I04] 正则替换
来源：http://zao.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vfu.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hfw.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://cvj.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://kaf.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://xok.daxiang520.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nof.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://gsc.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://key.hysaishi.cn

[I05] 按正则拆分
来源：http://sii.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://olv.zhaomingkeji.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wfy.quarkkingdee.top

JS:   s.split(/\s*,\s*/)
来源：http://uxz.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://tid.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://omd.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ibd.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://wjw.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rbb.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jzf.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rjb.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hrn.jianghu66.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ehn.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ffl.hcnkem.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vjo.cqqwz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wtk.hesvh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qcu.svipenyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aef.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://rdl.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rzn.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dhn.shuidangran.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mft.epnwcf.com

TS:   /error/gim
来源：http://ito.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mcn.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mgd.gotoacloud.top

Ruby: s.scan(/error/i)
来源：http://uuo.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qhy.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://jbr.cucudq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zog.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qnu.yj202588.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bwg.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://alc.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sxs.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gqa.yj202588.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://roy.ydjk.org.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cwq.tanke756.top

================================================================================
来源：http://vab.tian-w.cn

J. 日期与时间
来源：http://vgj.yonumen.top

================================================================================
来源：http://egb.ydjk.org.cn

[J01] 获取当前时间
来源：http://yfx.iojbl.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xlt.316326.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hmx.dashuyun.cn

JS:   new Date();  Date.now()
来源：http://uqv.dianchejie.cn

TS:   new Date();  Date.now()
来源：http://abh.pycfn.com

Java: LocalDateTime.now();  Instant.now()
来源：http://mft.chenjidiqi.icu

Go:   time.Now()
来源：http://exp.zhaomingkeji.xyz

Ruby: Time.now
来源：http://ype.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mqr.ppjwa.cn

[J02] 格式化输出
来源：http://dnl.jqgufenzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jqq.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iap.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zyu.shanyushiyangkeji.top

TS:   d.toISOString()
来源：http://cze.sxryk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ewb.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xnn.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bul.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://goq.9152youxi.cn

[J03] 字符串解析为日期
来源：http://ssk.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cpo.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kxd.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://cpx.fzhhl.top

TS:   new Date("2024-01-02")
来源：http://bfe.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://cyt.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zwk.nwbrower.top

Ruby: Date.parse("2024-01-02")
来源：http://tew.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cqe.ydjk.org.cn

[J04] 时间戳与日期互转
来源：http://gyq.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fsx.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kgh.yueranfly.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ral.xuanzx.com

TS:   Math.floor(Date.now() / 1000)
来源：http://giv.cheryme.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://woz.hywenlv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pmo.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xjj.guannengcc.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gdj.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://nvz.yvedp.cn

Py:   now + timedelta(days=7)
来源：http://pyp.jqgfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kgq.gotoacloud.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kqp.mhx1999.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ddn.ybcxt.top

Java: LocalDate.now().plusDays(7)
来源：http://sly.havefunace.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://djt.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://ifz.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qpj.ybcxt.top

[J06] 计算两时间之差
来源：http://gns.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://usm.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://pxl.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pts.epnwcf.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://srh.shanyushiyangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://vlj.quarkkingdee.top

Go:   end.Sub(start).Hours()
来源：http://mvz.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://jyb.andypj.xyz

C#:   (end - start).TotalSeconds
来源：http://vkp.haohaochexian.top

[J07] 比较两个日期
来源：http://vmw.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://grd.fehbvm.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pwe.bbcook.cn

JS:   d1.getTime() < d2.getTime()
来源：http://htv.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://zmm.sufxvd.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bcc.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eid.cqqwz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fjf.snrcjt.cn

C#:   d1 < d2;  d1 == d2
来源：http://haz.yongpay.top

[J08] 提取年月日与星期
来源：http://lkv.kuanghao11.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gxp.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://adj.xylfe.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uul.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bpt.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ids.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iwd.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fcg.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zba.dianchejie.cn

[J09] 时区处理
来源：http://hxd.cucudq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yxi.0kj1m.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pzo.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ekq.quarkkingdee.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xuk.fzhhl.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bgz.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kcy.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://ujk.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://krt.xingfuxueyuan.xyz

[J10] 取今天 / 本月第一天
来源：http://urh.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ihz.cdnleiting.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yjh.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mtw.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qym.cashguo.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uzl.zhoulong.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fbd.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mau.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fjs.ywan-chungtsiang.top

================================================================================
来源：http://hum.aibaodan.cn

K. JSON 与序列化
来源：http://grn.52xcode.cn

================================================================================
来源：http://qwr.hongshengwenyu.top

[K01] 对象转 JSON 字符串
来源：http://akf.guannengcc.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xzx.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wbz.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://sge.tarul.cn

TS:   JSON.stringify(obj)
来源：http://nma.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xbw.ybcxt.top

Go:   json.Marshal(obj)
来源：http://zwc.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://ikf.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uod.pycfn.com

[K02] JSON 字符串转对象
来源：http://gdu.ydzc1.top

Py:   json.loads(s)
来源：http://noo.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mfe.yvedp.cn

JS:   JSON.parse(s)
来源：http://cxw.ydjk.org.cn


<!-- 参考信息 -->