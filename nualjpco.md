代发 wailian999

PHP:  get_object_vars($obj);
来源：http://pgg.tarul.cn

JS:   Object.entries(obj)
来源：http://hco.yj20258.top

TS:   Object.entries(obj)
来源：http://heu.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ztp.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dbh.sufxvd.cn

Ruby: obj.instance_variables
来源：http://luj.shangyingyoupin.top

C#:   // 用反射或 System.Text.Json
来源：http://dum.yanxiufei.cn

================================================================================
来源：http://nvb.hnxiangtu.top

H. 异常与错误处理
来源：http://yvr.jinghuilouyu.cn

================================================================================
来源：http://pbt.xuanzx.com

[H01] try / catch 基础
来源：http://gwn.fzhhl.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vhb.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pkn.ydzc1.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xfm.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://izd.iojbl.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://guf.jqgfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yma.guowangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gug.sufxvd.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zhf.vehdjk.com

[H02] finally / ensure 收尾
来源：http://enx.tanke756.top

Py:   try: f()⏎finally: cleanup()
来源：http://ddd.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://rqx.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oan.cashguo.top

TS:   try { f(); } finally { cleanup(); }
来源：http://din.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wef.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jsy.yangfankeji.com

Ruby: begin; f; ensure; cleanup; end
来源：http://lqa.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mno.jqgufenzy.top

[H03] 主动抛出异常
来源：http://gjf.yongpay.top

Py:   raise ValueError("错误信息")
来源：http://xlc.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://czq.shanyushiyangtech.top

JS:   throw new Error("错误信息");
来源：http://syw.ctjpmb.com

TS:   throw new Error("错误信息");
来源：http://aum.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mqw.zhongyouzk.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tyg.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://keq.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://otr.sufxvd.cn

[H04] 自定义异常类型
来源：http://ryc.snrcjt.cn

Py:   class MyError(Exception): pass
来源：http://shl.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dwk.shuidangran.top

JS:   class MyError extends Error {}
来源：http://oea.0kj1m.cn

TS:   class MyError extends Error {}
来源：http://zpx.sufxvd.cn

Java: class MyException extends RuntimeException {}
来源：http://ric.dashuyun.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xyr.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://viq.zhaomingkeji.xyz

C#:   class MyException : Exception {}
来源：http://paa.redwolf501.top

[H05] 捕获特定类型
来源：http://cen.gaohongyu789.top

Py:   except ValueError as e:
来源：http://yyo.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qpo.yueranfly.top

JS:   if (e instanceof TypeError) {}
来源：http://omp.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://hcz.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://wvk.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dfk.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://fev.epnwcf.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dmh.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://efn.daria6918.cn

Py:   value = d.get("k") or default
来源：http://crr.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rbz.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://mzh.zdqjudy.top

TS:   obj?.a?.b;  d ?? default
来源：http://xxo.gotoacloud.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lqg.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zxq.shzxlz.cn

Ruby: d&.dig(:a, :b)
来源：http://upo.zhixingplan.top

C#:   obj?.A?.B ?? default
来源：http://dox.hfpthk.cn

[H07] 断言
来源：http://uno.meibo888.top

Py:   assert x > 0, "必须为正"
来源：http://jpx.nwbrower.top

PHP:  assert($x > 0);
来源：http://agx.hfpthk.cn

JS:   console.assert(x > 0);
来源：http://ozg.jinqigfzy.top

TS:   console.assert(x > 0);
来源：http://sun.ppjwa.cn

Java: assert x > 0 : "必须为正";
来源：http://hgx.zhixingplan.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tcf.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://eqg.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://xrx.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://wnr.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://kip.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://prr.cqqwz.cn

JS:   e.message;  e.stack
来源：http://gfy.pengpengdd.cyou

TS:   e instanceof Error ? e.message : String(e)
来源：http://mbo.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://iwq.zhengqikj.top

Go:   err.Error()
来源：http://zsq.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://tdr.feifeiyinyue.top

C#:   e.Message;  e.StackTrace
来源：http://azc.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://whv.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lmy.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://poy.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zzy.haohaochexian.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zpl.jlsjyb.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ixp.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://avk.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://lnw.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://qyd.ywan-chungtsiang.top

[H10] 资源自动释放
来源：http://qnq.sxryk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fqd.zhixingplan.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mhw.9152youxi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dnr.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kne.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://urx.ivvv.top

Go:   defer f.Close()
来源：http://mim.yvedp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bkq.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gno.xinyue.icu

================================================================================
来源：http://gug.hammf.cn

I. 正则表达式
来源：http://zjl.ppjwa.cn

================================================================================
来源：http://aas.hysaishi.cn

[I01] 判断是否匹配
来源：http://faq.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hyz.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mml.andypj.xyz

JS:   /\d+/.test(s)
来源：http://wot.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://hbu.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ynj.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://spv.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://sdz.fengsongda.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://foj.52xcode.cn

[I02] 提取所有匹配
来源：http://grn.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://nmt.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gxp.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://clj.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://jpp.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lnz.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lwk.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://wpi.hnxiangtu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://faw.ivvv.top

[I03] 提取捕获分组
来源：http://brp.uphjek.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vbb.yuanzhike.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vwv.chenjidiqi.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pfx.fanxiaobao.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kya.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sew.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://icy.hywenlv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ryc.yueranfly.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bgp.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://vtl.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pcz.ehwqpu.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gif.xylfe.cn

JS:   s.replace(/\d+/g, "#")
来源：http://frg.pycfn.com

TS:   s.replace(/\d+/g, "#")
来源：http://gon.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://ebp.quarkkingdee.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qcn.ctjpmb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://fjd.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://msn.9152youxi.cn

[I05] 按正则拆分
来源：http://huu.zycfv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zds.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hpn.316326.xyz

JS:   s.split(/\s*,\s*/)
来源：http://njy.ivvv.top

TS:   s.split(/\s*,\s*/)
来源：http://sit.hnqzz.top

Java: s.split("\\s*,\\s*")
来源：http://qpo.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bpd.tarul.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nkp.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://opc.wangdashe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xki.smart0.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ehq.fzhhl.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hyg.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mqi.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kes.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ibx.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mzv.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wfk.jqgufenzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lck.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://byx.iojbl.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vjr.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hwk.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://htw.epnwcf.com

TS:   /error/gim
来源：http://ozq.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kkh.shanyushiyangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qyo.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://nyp.yj20258.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dyc.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://spu.fanxiaobao.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ndt.vqdsnc.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gtf.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jex.hnqzz.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dro.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rmb.dashuyun.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dfc.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xxm.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qry.ctjpmb.com

================================================================================
来源：http://wzm.snrcjt.cn

J. 日期与时间
来源：http://mpx.hesvh.cn

================================================================================
来源：http://jif.gaohongyu789.top

[J01] 获取当前时间
来源：http://fqe.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://btf.wangshuangyany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tya.hongshengwenyu.top

JS:   new Date();  Date.now()
来源：http://qkz.wangshuangyany.cn

TS:   new Date();  Date.now()
来源：http://yge.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nbr.yfazqb.com

Go:   time.Now()
来源：http://aqg.guannengcc.top

Ruby: Time.now
来源：http://lel.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://njm.hywenlv.cn

[J02] 格式化输出
来源：http://pft.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zix.vqdsnc.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xwu.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rai.shangyingyoupin.top

TS:   d.toISOString()
来源：http://cnw.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iex.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pnh.yangfankeji.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tmy.hywenlv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hbw.nanxuanxn.top

[J03] 字符串解析为日期
来源：http://hei.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nnb.shanyushiyangtech.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eur.fktsv.cn

JS:   new Date("2024-01-02")
来源：http://fgp.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://kez.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://vfg.guannengcc.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qel.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://svd.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kwl.daria6918.cn

[J04] 时间戳与日期互转
来源：http://fkv.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://njm.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ibt.feifeiyinyue.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tqw.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lqu.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uph.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nul.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kqs.fktsv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jzm.zhijiandao.cn

[J05] 时间加减（加 7 天）
来源：http://pvl.havefunace.top

Py:   now + timedelta(days=7)
来源：http://aiq.smart0.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://nrj.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dnm.zycfv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nus.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://wab.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ete.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://rfz.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://sqz.yuxming.cn

[J06] 计算两时间之差
来源：http://vms.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://raj.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://wfl.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pfy.bjfxy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tfz.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nmr.fehbvm.com

Go:   end.Sub(start).Hours()
来源：http://tav.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://jxi.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://ayc.haohaochexian.top

[J07] 比较两个日期
来源：http://vqv.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://fai.zhijiandao.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uwp.yanxiufei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ixn.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bqp.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vmt.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hwl.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://dae.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://mad.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://dyo.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lyz.xylfe.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tzp.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://osb.yvedp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://saq.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ydz.jiagoushi.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lbh.svipenyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ccw.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wrn.vehdjk.com

[J09] 时区处理
来源：http://tsw.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://geq.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fbf.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fcd.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nas.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uyd.jinghuilouyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ber.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ilh.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qji.hcnkem.com

[J10] 取今天 / 本月第一天
来源：http://imj.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://iss.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tum.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yue.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kil.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fgo.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://stc.bbcook.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mmq.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kbh.zhengqikj.top

================================================================================
来源：http://nsb.jqgfzy.top

K. JSON 与序列化
来源：http://rfi.cashguo.top

================================================================================
来源：http://uso.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://cov.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ehq.jyoumei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://scd.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://nca.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://owj.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fux.meibo888.top

Go:   json.Marshal(obj)
来源：http://pzx.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://gbt.bbcook.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iit.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://qnm.dashuyun.cn

Py:   json.loads(s)
来源：http://bwg.cdnleiting.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rhj.ivvv.top

JS:   JSON.parse(s)
来源：http://goh.iojbl.cn

TS:   JSON.parse(s)
来源：http://mkt.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cxe.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://mjs.fktsv.cn

Ruby: JSON.parse(s)
来源：http://jkp.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fic.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://ggl.cheryme.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lms.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cmw.ctjpmb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://fwt.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hfn.fktsv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fxa.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gdj.yonumen.top

Ruby: JSON.pretty_generate(obj)
来源：http://xev.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://egz.yuanzhike.top

[K04] 读取 JSON 文件
来源：http://dek.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ffz.aibaodan.cn


<!-- 参考信息 -->