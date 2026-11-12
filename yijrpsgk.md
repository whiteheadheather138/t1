代发 wailian999

PHP:  get_object_vars($obj);
来源：http://ywb.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://ppb.hysaishi.cn

TS:   Object.entries(obj)
来源：http://mbl.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vnc.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://tet.birdmap.top

Ruby: obj.instance_variables
来源：http://vld.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://mwj.hfpthk.cn

================================================================================
来源：http://zir.zhengqikj.top

H. 异常与错误处理
来源：http://urg.birdmap.top

================================================================================
来源：http://mme.yfazqb.com

[H01] try / catch 基础
来源：http://szo.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cen.redwolf501.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://khr.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nva.yangfankeji.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vtp.jyoumei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hji.shuidangran.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ido.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ahd.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sii.yangfankeji.com

[H02] finally / ensure 收尾
来源：http://erz.yj20258.top

Py:   try: f()⏎finally: cleanup()
来源：http://jof.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nqm.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://mtf.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ikx.vehdjk.com

Java: try { f(); } finally { cleanup(); }
来源：http://vfp.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yly.zhijiandao.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://scl.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://leh.xinyue.icu

[H03] 主动抛出异常
来源：http://wso.nanxuanxn.top

Py:   raise ValueError("错误信息")
来源：http://gag.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ztm.sysykeji.top

JS:   throw new Error("错误信息");
来源：http://ioj.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://fyj.xziqi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ivu.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tpj.sysykeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://joa.shanyushiyangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://upc.hysaishi.cn

[H04] 自定义异常类型
来源：http://exf.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://png.yuxming.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dwl.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://rzp.fengsongda.top

TS:   class MyError extends Error {}
来源：http://mhd.zhongyouzk.top

Java: class MyException extends RuntimeException {}
来源：http://zca.svipenyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fgp.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://ruz.shzxlz.cn

C#:   class MyException : Exception {}
来源：http://twh.wangdashe.top

[H05] 捕获特定类型
来源：http://aqg.316326.xyz

Py:   except ValueError as e:
来源：http://skh.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mdy.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://wez.svipenyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://kxm.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://vfk.yonumen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rne.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://yvs.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aqx.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://qjo.fzhhl.top

Py:   value = d.get("k") or default
来源：http://dts.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://qoi.zdbjq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kfr.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wil.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eag.hcnkem.com

Go:   if v, ok := m["k"]; ok { }
来源：http://qnz.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://fmp.vqdsnc.cn

C#:   obj?.A?.B ?? default
来源：http://dqz.cashguo.top

[H07] 断言
来源：http://zvg.kuanghao11.cn

Py:   assert x > 0, "必须为正"
来源：http://rpd.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://hlv.cheryme.top

JS:   console.assert(x > 0);
来源：http://nkr.hywenlv.cn

TS:   console.assert(x > 0);
来源：http://pdu.ehwqpu.com

Java: assert x > 0 : "必须为正";
来源：http://gdt.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tnk.jyoumei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gyz.hongshengwenyu.top

C#:   Debug.Assert(x > 0);
来源：http://asi.yueranfly.top

[H08] 获取错误信息与堆栈
来源：http://jcy.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://nes.dianchejie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ofp.hesvh.cn

JS:   e.message;  e.stack
来源：http://ncs.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sry.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qxx.jqgufenzy.top

Go:   err.Error()
来源：http://gaf.zhaomingkeji.xyz

Ruby: e.message;  e.backtrace
来源：http://css.yanxiufei.cn

C#:   e.Message;  e.StackTrace
来源：http://iux.vehdjk.com

[H09] 带错误码的异常
来源：http://mlq.quarkkingdee.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mzw.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pou.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xse.ctjpmb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sco.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ukz.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zqt.uphjek.com

Ruby: raise MyError.new("fail", 500)
来源：http://lta.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://uhv.52xcode.cn

[H10] 资源自动释放
来源：http://wau.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lxt.0kj1m.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jhl.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uoe.smart0.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qbu.gogol.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vyo.ydzc1.top

Go:   defer f.Close()
来源：http://hks.hywenlv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lgu.zhijiandao.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yfj.fengsongda.top

================================================================================
来源：http://lyf.snrcjt.cn

I. 正则表达式
来源：http://abf.jyoumei.cn

================================================================================
来源：http://cwv.chenzaomai.com

[I01] 判断是否匹配
来源：http://qpy.hfpthk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dmh.fengsongda.top

PHP:  preg_match('/\d+/', $s);
来源：http://tds.wangdashe.top

JS:   /\d+/.test(s)
来源：http://muz.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://ops.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tcv.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gvz.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://lcl.xinyue.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lqg.yj20258888.top

[I02] 提取所有匹配
来源：http://hfu.cheryme.top

Py:   re.findall(r"\d+", s)
来源：http://yjq.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tbd.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://beg.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://eqv.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tjj.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ewp.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://uyf.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vlq.xuanzx.com

[I03] 提取捕获分组
来源：http://yaf.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eiw.yvedp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ype.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nkh.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ymo.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pri.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kuk.sjlbkw.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vyu.hongshengwenyu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jyz.ehwqpu.com

[I04] 正则替换
来源：http://mnt.bbcook.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ifp.cheryme.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kka.iojbl.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lma.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://toz.ydjk.org.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rsv.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vlb.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://olo.ybcxt.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blw.52xcode.cn

[I05] 按正则拆分
来源：http://btt.pengpengdd.cyou

Py:   re.split(r"\s*,\s*", s)
来源：http://vgw.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://umt.nanxinkj.top

JS:   s.split(/\s*,\s*/)
来源：http://ctg.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://oqe.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://tvo.fengsongda.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tsk.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://gsi.tian-w.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qhe.xingfuxueyuan.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ixp.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uen.vehdjk.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nwe.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cva.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pxz.kuanghao11.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dyf.zhixingplan.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cwo.chenjidiqi.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lzx.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uli.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://feo.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wvs.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rtx.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zdr.cdnleiting.top

TS:   /error/gim
来源：http://bbd.bjfxy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rrd.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mpi.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://qoq.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://psv.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://icx.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://juv.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oqq.nanxinkj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tqr.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://csl.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bnw.feifeiyinyue.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fpi.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://itq.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://voz.tarul.cn

================================================================================
来源：http://rbx.zhongyouzk.top

J. 日期与时间
来源：http://gvn.cucudq.cn

================================================================================
来源：http://zvw.yanxiufei.cn

[J01] 获取当前时间
来源：http://lps.hfpthk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qwk.yueranfly.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pdq.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://djv.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://bqx.iojbl.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ctv.fehbvm.com

Go:   time.Now()
来源：http://qnb.cdnleiting.top

Ruby: Time.now
来源：http://kna.haohaochexian.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wir.snrcjt.cn

[J02] 格式化输出
来源：http://xxq.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vlu.c1oappe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wxb.yvedp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://las.0kj1m.cn

TS:   d.toISOString()
来源：http://hpc.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yuj.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uua.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uhg.ydjk.org.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sgv.xziqi.cn

[J03] 字符串解析为日期
来源：http://rex.shuidangran.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://elk.ehwqpu.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rxf.fzhhl.top

JS:   new Date("2024-01-02")
来源：http://eyi.uphjek.com

TS:   new Date("2024-01-02")
来源：http://lzg.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://xpf.jinqigufen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ung.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://qbu.hnxiangtu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wby.hywenlv.cn

[J04] 时间戳与日期互转
来源：http://rqe.fengsongda.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lrm.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tam.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fws.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hhm.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://afv.birdmap.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ewp.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://izg.ctjpmb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zok.nanxuanxn.top

[J05] 时间加减（加 7 天）
来源：http://sgz.gaohongyu789.top

Py:   now + timedelta(days=7)
来源：http://iop.chenjidiqi.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://fdb.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bnj.zdbjq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gwx.jqgfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://uls.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rwf.ppjwa.cn

Ruby: Time.now + 7 * 86400
来源：http://jgb.guannengcc.top

C#:   DateTime.Now.AddDays(7)
来源：http://hnn.meibo888.top

[J06] 计算两时间之差
来源：http://wam.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://iis.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://flb.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://crx.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mac.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zik.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://ead.zhixingplan.top

Ruby: end - start                 # 返回秒数
来源：http://opq.hfpthk.cn

C#:   (end - start).TotalSeconds
来源：http://mqg.svipenyu.cn

[J07] 比较两个日期
来源：http://mtd.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://err.tarul.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lxu.shuidangran.top

JS:   d1.getTime() < d2.getTime()
来源：http://vci.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ere.chenzaomai.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hrr.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lrj.sufxvd.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pwl.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://for.tarul.cn

[J08] 提取年月日与星期
来源：http://nsn.yangfankeji.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mlt.quarkkingdee.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tql.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://anz.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yol.yuanzhike.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ldq.sweek.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xuy.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bhp.uphjek.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bkq.aizwys.cn

[J09] 时区处理
来源：http://ope.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cfj.feifeiyinyue.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ajw.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://csa.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xxb.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jga.zhengqikj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jcn.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vwc.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lav.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://xbr.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://bgn.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mii.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nyo.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kjx.xylfe.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qmi.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ani.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pra.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ieh.52xcode.cn

================================================================================
来源：http://eyy.cdnleiting.top

K. JSON 与序列化
来源：http://khf.yueranfly.top

================================================================================
来源：http://jlr.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://mvg.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bbu.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kdi.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://axo.daxiang520.top

TS:   JSON.stringify(obj)
来源：http://fvm.yj202588.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ims.xingfuxueyuan.xyz

Go:   json.Marshal(obj)
来源：http://qrt.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://hir.chenlongwang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zae.pycfn.com

[K02] JSON 字符串转对象
来源：http://evr.wangshuangyany.cn

Py:   json.loads(s)
来源：http://gfo.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ryn.zhengqikj.top

JS:   JSON.parse(s)
来源：http://udo.dianchejie.cn

TS:   JSON.parse(s)
来源：http://jbm.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eqm.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://pzw.vehdjk.com

Ruby: JSON.parse(s)
来源：http://ahq.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vsd.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://zux.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xhm.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vux.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://aaz.fengsongda.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nvx.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wbl.fengsongda.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pnz.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vfx.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vkl.jqgfzy.top

[K04] 读取 JSON 文件
来源：http://mji.yonumen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fkg.zhoulong.xyz


<!-- 参考信息 -->