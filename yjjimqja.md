代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://goc.tianlin.xyz

Java: record User(String name, int age) {}
来源：http://ikd.zhongyouzk.top

Go:   type User struct { Name string; Age int }
来源：http://jxc.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dby.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://lmq.ydzc1.top

[G15] 枚举
来源：http://mvi.hesvh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mzo.0kj1m.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zsq.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eoi.sxryk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fhl.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://buj.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jbk.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://etu.shuidangran.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xrp.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://oxr.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dca.meibo888.top

PHP:  get_object_vars($obj);
来源：http://kqa.shzxlz.cn

JS:   Object.entries(obj)
来源：http://vun.jiagoushi.top

TS:   Object.entries(obj)
来源：http://khh.xingfuxueyuan.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zjy.aizwys.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rwc.tanke756.top

Ruby: obj.instance_variables
来源：http://tgx.zhoulong.xyz

C#:   // 用反射或 System.Text.Json
来源：http://ugx.gaohongyu789.top

================================================================================
来源：http://als.fengsongda.top

H. 异常与错误处理
来源：http://rep.sxryk.cn

================================================================================
来源：http://mro.hongshengwenyu.top

[H01] try / catch 基础
来源：http://bzl.yj20258888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://naq.vqdsnc.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pqt.ydzc1.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://coq.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xqp.zhongyouzk.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hta.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hea.ydzc1.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dmf.hysaishi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://umm.ydjk.org.cn

[H02] finally / ensure 收尾
来源：http://coi.wangshuangyany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://exw.dianchejie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iwk.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://okz.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hvc.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://ltc.sysykeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bnq.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lsp.guowangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nue.jiagoushi.top

[H03] 主动抛出异常
来源：http://geg.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://ete.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hpp.ivvv.top

JS:   throw new Error("错误信息");
来源：http://ebi.zhoulong.xyz

TS:   throw new Error("错误信息");
来源：http://hrf.hnqzz.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mqh.jiagoushi.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mdx.cucudq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hbl.andypj.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://ymu.iojbl.cn

[H04] 自定义异常类型
来源：http://yqv.shanyushiyangtech.top

Py:   class MyError(Exception): pass
来源：http://gdt.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://klu.uphjek.com

JS:   class MyError extends Error {}
来源：http://bkl.vqdsnc.cn

TS:   class MyError extends Error {}
来源：http://yyp.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://ibf.cashguo.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://stc.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://jqu.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://sjv.zhixingplan.top

[H05] 捕获特定类型
来源：http://emj.yj20258.top

Py:   except ValueError as e:
来源：http://owx.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ufh.daxiang520.top

JS:   if (e instanceof TypeError) {}
来源：http://ggo.52xcode.cn

TS:   if (e instanceof TypeError) {}
来源：http://wnu.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://swg.jinqigfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ana.shzxlz.cn

Ruby: rescue ArgumentError => e
来源：http://coj.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yfw.sxryk.cn

[H06] 可选值 / 空值安全访问
来源：http://hqt.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://phq.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wjv.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://chy.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://zjg.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bcv.ydjk.org.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vvu.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://jgk.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://met.yangfankeji.com

[H07] 断言
来源：http://sla.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://wdg.zdqjudy.top

PHP:  assert($x > 0);
来源：http://gnu.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://wqv.fzhhl.top

TS:   console.assert(x > 0);
来源：http://pwo.ppjwa.cn

Java: assert x > 0 : "必须为正";
来源：http://anp.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dtr.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://ctc.fengsongda.top

C#:   Debug.Assert(x > 0);
来源：http://wiz.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://dbc.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://qow.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gwr.hysaishi.cn

JS:   e.message;  e.stack
来源：http://mdh.sysykeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gct.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kqd.vehdjk.com

Go:   err.Error()
来源：http://enm.9152youxi.cn

Ruby: e.message;  e.backtrace
来源：http://qca.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://ykt.tianlin.xyz

[H09] 带错误码的异常
来源：http://sfy.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xid.meibo888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pqv.yfazqb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qcb.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zkh.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xjq.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uii.tianlin.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://mbm.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://sac.guowangkeji.top

[H10] 资源自动释放
来源：http://zon.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://fik.ctjpmb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cyg.shanyushiyangtech.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fri.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ccv.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nxr.hfpthk.cn

Go:   defer f.Close()
来源：http://cri.jinqigfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vrc.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mhl.ydjk.org.cn

================================================================================
来源：http://abn.iojbl.cn

I. 正则表达式
来源：http://xip.guannengcc.top

================================================================================
来源：http://ypz.aizwys.cn

[I01] 判断是否匹配
来源：http://gta.xinyue.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oeq.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jjo.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://bmb.aizwys.cn

TS:   /\d+/.test(s)
来源：http://cle.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ous.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fou.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://xwf.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bmc.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://weq.xylfe.cn

Py:   re.findall(r"\d+", s)
来源：http://vpe.tanke756.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ucp.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tmg.birdmap.top

TS:   s.match(/\d+/g)
来源：http://rwa.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ggt.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jcw.shuidangran.top

Ruby: s.scan(/\d+/)
来源：http://dnz.smart0.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cat.shzxlz.cn

[I03] 提取捕获分组
来源：http://tiw.yfazqb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gwf.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sst.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qhs.ywan-chungtsiang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kgp.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://orp.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ocl.fehbvm.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bbb.zdbjq.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tlk.sufxvd.cn

[I04] 正则替换
来源：http://vav.haohaochexian.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hnf.yongpay.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nft.fktsv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://shv.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://djr.iojbl.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ppf.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fac.haohaochexian.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vio.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zwx.guannengcc.top

[I05] 按正则拆分
来源：http://cyr.zhaomingkeji.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://odw.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sxu.vqdsnc.cn

JS:   s.split(/\s*,\s*/)
来源：http://woj.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://hss.ehwqpu.com

Java: s.split("\\s*,\\s*")
来源：http://htw.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://flz.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://dkw.xziqi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://isp.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zaa.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ekk.nanxinkj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mya.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hhh.uphjek.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vth.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vqj.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ktn.cashguo.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wdg.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://geo.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://gql.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qha.jinqigfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://njr.shanyushiyangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vbe.zycfv.cn

TS:   /error/gim
来源：http://vqz.nanxinkj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uqx.zhoulong.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://udq.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://bqe.cucudq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vfl.hammf.cn

[I08] 贪婪与非贪婪匹配
来源：http://yiu.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bxv.sysykeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nsw.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jhr.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qvw.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://qim.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ymr.gzhubu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://amk.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dfq.cucudq.cn

================================================================================
来源：http://div.tianlin.xyz

J. 日期与时间
来源：http://dfc.cdnleiting.top

================================================================================
来源：http://ryc.fehbvm.com

[J01] 获取当前时间
来源：http://uma.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jfr.daria6918.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zoa.c1oappe.top

JS:   new Date();  Date.now()
来源：http://jgw.yvedp.cn

TS:   new Date();  Date.now()
来源：http://czz.sufxvd.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ojk.sjlbkw.cn

Go:   time.Now()
来源：http://nih.hesvh.cn

Ruby: Time.now
来源：http://wpe.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ska.hfpthk.cn

[J02] 格式化输出
来源：http://khq.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dcv.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kao.vehdjk.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yjj.tarul.cn

TS:   d.toISOString()
来源：http://vik.shangyingyoupin.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zpl.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pse.guannengcc.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://own.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pyz.nwbrower.top

[J03] 字符串解析为日期
来源：http://plb.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dny.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fen.haohaochexian.top

JS:   new Date("2024-01-02")
来源：http://zgf.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://puf.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://piz.fanxiaobao.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fve.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://rkt.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yxx.hcnkem.com

[J04] 时间戳与日期互转
来源：http://apf.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ayn.uphjek.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lhd.jinyuanbaomall.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ouw.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zjx.nanxuanxn.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sgt.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://itp.yj20258.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://frk.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wal.quarkkingdee.top

[J05] 时间加减（加 7 天）
来源：http://vaq.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://qhc.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://aje.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bfu.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pmt.ydjk.org.cn

Java: LocalDate.now().plusDays(7)
来源：http://ccd.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hrm.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://ptw.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qfi.hcnkem.com

[J06] 计算两时间之差
来源：http://ijs.feifeiyinyue.top

Py:   (end - start).total_seconds()
来源：http://slp.hysaishi.cn

PHP:  $end->diff($start)->days;
来源：http://fde.cucudq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://leh.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://txs.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ezd.bbcook.cn

Go:   end.Sub(start).Hours()
来源：http://fyp.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://zdr.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://emz.cashguo.top

[J07] 比较两个日期
来源：http://vfc.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://mzo.yvedp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mjy.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lgc.chenjidiqi.icu

TS:   d1.getTime() < d2.getTime()
来源：http://fxh.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mxu.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gen.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://vop.shangyingyoupin.top

C#:   d1 < d2;  d1 == d2
来源：http://zjs.birdmap.top

[J08] 提取年月日与星期
来源：http://ddx.ctjpmb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hbl.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yge.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ydj.nanxinkj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oqa.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wwf.feifeiyinyue.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vrx.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zyi.xingfuxueyuan.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://osb.shuidangran.top

[J09] 时区处理
来源：http://has.bjfxy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vdp.mhx1999.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ewv.hammf.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rjh.tianlin.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jql.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ktj.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mfm.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kgy.gogol.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uyy.nwbrower.top

[J10] 取今天 / 本月第一天
来源：http://apf.yj202588.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ygf.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zfj.gzhubu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sgi.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lje.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ivq.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hpa.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wgf.ydzc1.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wao.aibaodan.cn

================================================================================
来源：http://qtn.tian-w.cn

K. JSON 与序列化
来源：http://bvb.zycfv.cn

================================================================================
来源：http://acl.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://pnv.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lcw.birdmap.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nrn.yj20258888.top

JS:   JSON.stringify(obj)
来源：http://hjl.hammf.cn

TS:   JSON.stringify(obj)
来源：http://atn.sweek.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ppa.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://ykz.yongpay.top

Ruby: obj.to_json                                     // require "json"
来源：http://khh.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wsw.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://htt.hfpthk.cn

Py:   json.loads(s)
来源：http://quc.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://asc.havefunace.top

JS:   JSON.parse(s)
来源：http://zcg.redwolf501.top


<!-- 参考信息 -->