代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://slh.tian-w.cn

Ruby: obj.instance_variables
来源：http://wkq.sysykeji.top

C#:   // 用反射或 System.Text.Json
来源：http://gzh.tianlin.xyz

================================================================================
来源：http://vzm.xuetiantiany.cn

H. 异常与错误处理
来源：http://ezf.quarkkingdee.top

================================================================================
来源：http://xbm.hammf.cn

[H01] try / catch 基础
来源：http://tju.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qqq.ybcxt.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fdt.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zfh.yangfankeji.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dkn.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aju.wangdashe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nai.c1oappe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://arx.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iwi.smart0.xyz

[H02] finally / ensure 收尾
来源：http://wsz.guowangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://tog.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nme.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://aar.vehdjk.com

TS:   try { f(); } finally { cleanup(); }
来源：http://cfx.tarul.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tqy.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://apf.pycfn.com

Ruby: begin; f; ensure; cleanup; end
来源：http://bte.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bxd.vqdsnc.cn

[H03] 主动抛出异常
来源：http://wqe.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://zaa.epnwcf.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zdo.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://vfg.jinqigufen.top

TS:   throw new Error("错误信息");
来源：http://fxs.hnqzz.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://aef.hfpthk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bbn.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gis.cashguo.top

C#:   throw new ArgumentException("错误信息");
来源：http://hbe.cheryme.top

[H04] 自定义异常类型
来源：http://dsv.yonumen.top

Py:   class MyError(Exception): pass
来源：http://xaf.ydzc1.top

PHP:  class MyError extends RuntimeException {}
来源：http://fww.daxiang520.top

JS:   class MyError extends Error {}
来源：http://mel.xuanzx.com

TS:   class MyError extends Error {}
来源：http://hfz.9152youxi.cn

Java: class MyException extends RuntimeException {}
来源：http://xgs.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sgl.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://nti.hcnkem.com

C#:   class MyException : Exception {}
来源：http://dyv.cdnleiting.top

[H05] 捕获特定类型
来源：http://twa.guannengcc.top

Py:   except ValueError as e:
来源：http://lko.yj20258.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iro.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://rtt.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://ezm.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://lgj.9152youxi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vde.yonumen.top

Ruby: rescue ArgumentError => e
来源：http://vqm.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zyn.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://vsz.aizwys.cn

Py:   value = d.get("k") or default
来源：http://pvc.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://crm.ydjk.org.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nmi.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://qsk.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://atw.gotoacloud.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vaq.ydzc1.top

Ruby: d&.dig(:a, :b)
来源：http://okx.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://iyt.ybcxt.top

[H07] 断言
来源：http://omg.gogol.net.cn

Py:   assert x > 0, "必须为正"
来源：http://hrb.xziqi.cn

PHP:  assert($x > 0);
来源：http://ott.yj202588.top

JS:   console.assert(x > 0);
来源：http://gdk.fanxiaobao.xyz

TS:   console.assert(x > 0);
来源：http://zxe.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://ncz.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nfu.hesvh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iof.zdqjudy.top

C#:   Debug.Assert(x > 0);
来源：http://dex.pycfn.com

[H08] 获取错误信息与堆栈
来源：http://siy.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://egd.wangdashe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://swk.fanxiaobao.xyz

JS:   e.message;  e.stack
来源：http://rvg.9152youxi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://heq.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jkg.smart0.xyz

Go:   err.Error()
来源：http://xoq.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://qih.yueranfly.top

C#:   e.Message;  e.StackTrace
来源：http://sjz.aizwys.cn

[H09] 带错误码的异常
来源：http://uqk.zycfv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tng.zhengqikj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lcs.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pjz.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qwg.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cot.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nuh.yfazqb.com

Ruby: raise MyError.new("fail", 500)
来源：http://jpj.jinghuilouyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zbz.jyoumei.cn

[H10] 资源自动释放
来源：http://xgk.sxryk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ryx.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ijk.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://soa.jqgfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hbi.hongshengwenyu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vzv.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://mgd.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ngi.316326.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ehe.gogol.net.cn

================================================================================
来源：http://syw.redwolf501.top

I. 正则表达式
来源：http://wsl.jinqigfzy.top

================================================================================
来源：http://tic.smart0.xyz

[I01] 判断是否匹配
来源：http://jtw.fehbvm.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rgr.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://xyz.ehwqpu.com

JS:   /\d+/.test(s)
来源：http://ikr.fengsongda.top

TS:   /\d+/.test(s)
来源：http://byu.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rcx.iojbl.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uzt.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://mep.ybcxt.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gfp.gaohongyu789.top

[I02] 提取所有匹配
来源：http://iol.nanxinkj.top

Py:   re.findall(r"\d+", s)
来源：http://mwu.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rou.chenlongwang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://udm.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://sdz.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://phl.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ytk.tarul.cn

Ruby: s.scan(/\d+/)
来源：http://oxw.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ebh.cashguo.top

[I03] 提取捕获分组
来源：http://fnq.xylfe.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fqd.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://enx.nwbrower.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://plx.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wil.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mad.kuanghao11.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hso.xuetiantiany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vey.zdbjq.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dej.daxiang520.top

[I04] 正则替换
来源：http://uzd.vqdsnc.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rqx.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jfv.fktsv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tze.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://nmd.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cxm.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dqr.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://umq.tianlin.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wpp.aizwys.cn

[I05] 按正则拆分
来源：http://ulj.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zoq.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nln.dianchejie.cn

JS:   s.split(/\s*,\s*/)
来源：http://fkw.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://jhi.chenjidiqi.icu

Java: s.split("\\s*,\\s*")
来源：http://vxj.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fao.ppjwa.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pld.xziqi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wyk.ehwqpu.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pjj.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://awo.ctjpmb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hzx.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://efp.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tae.bbcook.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fwj.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fkl.kuanghao11.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xbd.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://muc.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://mhw.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cad.hammf.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vfo.andypj.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hnu.yvedp.cn

TS:   /error/gim
来源：http://zlg.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mpb.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kdy.9152youxi.cn

Ruby: s.scan(/error/i)
来源：http://rfy.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rgl.cucudq.cn

[I08] 贪婪与非贪婪匹配
来源：http://zmr.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dcn.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rcn.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ewq.ehwqpu.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gmy.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://vwi.cucudq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qqm.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mae.aibaodan.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ojz.wangshuangyany.cn

================================================================================
来源：http://ocb.yonumen.top

J. 日期与时间
来源：http://gon.wangdashe.top

================================================================================
来源：http://jez.chenjidiqi.icu

[J01] 获取当前时间
来源：http://oux.tanke756.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gpp.ctjpmb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zqe.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://qyb.andypj.xyz

TS:   new Date();  Date.now()
来源：http://art.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tlq.cashguo.top

Go:   time.Now()
来源：http://qny.daxiang520.top

Ruby: Time.now
来源：http://fsk.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://icb.haohaochexian.top

[J02] 格式化输出
来源：http://yip.uphjek.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hha.hammf.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gzx.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tck.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://ncb.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hwc.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://raw.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://czn.haohaochexian.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qtd.mhx1999.top

[J03] 字符串解析为日期
来源：http://iah.dashuyun.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xzk.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wux.yonumen.top

JS:   new Date("2024-01-02")
来源：http://zjw.9152youxi.cn

TS:   new Date("2024-01-02")
来源：http://eki.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jna.xuanzx.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gnz.vehdjk.com

Ruby: Date.parse("2024-01-02")
来源：http://nmb.xuetiantiany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hje.gaohongyu789.top

[J04] 时间戳与日期互转
来源：http://gzr.jinyuanbaomall.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lsn.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fni.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ejf.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qae.fzhhl.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eeb.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ofm.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cox.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://abl.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://zxa.zdqjudy.top

Py:   now + timedelta(days=7)
来源：http://tgj.chenjidiqi.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://hgp.cheryme.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gzk.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xdw.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://rjx.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mlt.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://lgo.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://cul.wangshuangyany.cn

[J06] 计算两时间之差
来源：http://mxv.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://bhz.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://big.mhx1999.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uwc.zhengqikj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xuz.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://nqe.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://gdv.jinyuanbaomall.cn

Ruby: end - start                 # 返回秒数
来源：http://yor.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://gag.iojbl.cn

[J07] 比较两个日期
来源：http://kuc.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://oww.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wsu.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://lkl.tanke756.top

TS:   d1.getTime() < d2.getTime()
来源：http://dzd.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lup.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ojg.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://jkc.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://uph.daxiang520.top

[J08] 提取年月日与星期
来源：http://jtc.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vux.yuxming.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fhe.sysykeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pvl.chenlongwang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cci.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zvg.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xrw.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ppg.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xhr.sysykeji.top

[J09] 时区处理
来源：http://lvz.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vgh.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lfu.ppjwa.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mej.yj20258.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ujp.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eyv.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rey.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rau.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hxx.zhiwuduotai.top

[J10] 取今天 / 本月第一天
来源：http://xak.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qpl.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yrj.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kvd.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://usa.guannengcc.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://flt.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nsw.shangyingyoupin.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hdb.xylfe.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qou.aibaodan.cn

================================================================================
来源：http://dsr.yvedp.cn

K. JSON 与序列化
来源：http://rgw.haohaochexian.top

================================================================================
来源：http://cwi.hnxiangtu.top

[K01] 对象转 JSON 字符串
来源：http://hmz.yuanzhike.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oml.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ulv.zhoulong.xyz

JS:   JSON.stringify(obj)
来源：http://lov.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://jeg.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lty.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://msa.redwolf501.top

Ruby: obj.to_json                                     // require "json"
来源：http://mvx.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://lvg.zhiwuduotai.top

[K02] JSON 字符串转对象
来源：http://nnu.jinqigfzy.top

Py:   json.loads(s)
来源：http://lyj.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lew.jiagoushi.top

JS:   JSON.parse(s)
来源：http://kgu.hammf.cn

TS:   JSON.parse(s)
来源：http://bgg.quarkkingdee.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zdk.sjlbkw.cn

Go:   json.Unmarshal(data, &v)
来源：http://vnm.yj20258.top

Ruby: JSON.parse(s)
来源：http://cid.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vms.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://hqr.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://guk.xylfe.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mgw.shanyushiyangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cgj.kuanghao11.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mok.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fhx.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://atu.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://cfs.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://twj.52xcode.cn

[K04] 读取 JSON 文件
来源：http://kyu.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zhi.yj20258.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xgj.xuetiantiany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jpd.ydjk.org.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nld.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rhq.yvedp.cn


<!-- 参考信息 -->