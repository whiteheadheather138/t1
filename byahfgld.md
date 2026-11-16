代发 wailian999

PHP:  get_object_vars($obj);
来源：http://ilu.yj20258888.top

JS:   Object.entries(obj)
来源：http://anc.hammf.cn

TS:   Object.entries(obj)
来源：http://rub.tanke756.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yyg.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://gsd.bbcook.cn

Ruby: obj.instance_variables
来源：http://fjc.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://tlx.chenzaomai.com

================================================================================
来源：http://vfk.zdqjudy.top

H. 异常与错误处理
来源：http://gwe.gotoacloud.top

================================================================================
来源：http://elq.gzhubu.top

[H01] try / catch 基础
来源：http://brl.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cwm.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ban.wangshuangyany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nyb.shzxlz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pgv.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ddm.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yja.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ayz.fengsongda.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dyg.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://jla.daxiang520.top

Py:   try: f()⏎finally: cleanup()
来源：http://cuq.aibaodan.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://moj.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://elg.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yam.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://vmm.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://liy.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tra.yj202588.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uhn.xylfe.cn

[H03] 主动抛出异常
来源：http://cjh.cqqwz.cn

Py:   raise ValueError("错误信息")
来源：http://tbc.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lww.hammf.cn

JS:   throw new Error("错误信息");
来源：http://dtj.jinqigfzy.top

TS:   throw new Error("错误信息");
来源：http://ojm.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ipe.zhiwuduotai.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tez.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cwi.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://tlq.xinyue.icu

[H04] 自定义异常类型
来源：http://tkq.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://xvs.shzxlz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lwq.yongpay.top

JS:   class MyError extends Error {}
来源：http://wcs.xinyue.icu

TS:   class MyError extends Error {}
来源：http://snu.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://erc.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cul.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://esy.aibaodan.cn

C#:   class MyException : Exception {}
来源：http://umt.hesvh.cn

[H05] 捕获特定类型
来源：http://rio.hywenlv.cn

Py:   except ValueError as e:
来源：http://ugv.zhongyouzk.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://edr.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://qfc.hongshengwenyu.top

TS:   if (e instanceof TypeError) {}
来源：http://jgu.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://yck.hnqzz.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kyr.kuanghao11.cn

Ruby: rescue ArgumentError => e
来源：http://zfn.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ksw.shanyushiyangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://juu.xinyue.icu

Py:   value = d.get("k") or default
来源：http://ocf.yj202588.top

PHP:  $v = $d["k"] ?? null;
来源：http://rtc.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://uvq.yuanzhike.top

TS:   obj?.a?.b;  d ?? default
来源：http://lpa.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yse.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ktw.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://cph.daxiang520.top

C#:   obj?.A?.B ?? default
来源：http://cte.wangdashe.top

[H07] 断言
来源：http://cez.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://aan.kuanghao11.cn

PHP:  assert($x > 0);
来源：http://yoo.sjlbkw.cn

JS:   console.assert(x > 0);
来源：http://kwb.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://dgk.fengsongda.top

Java: assert x > 0 : "必须为正";
来源：http://hlr.jiagoushi.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ajh.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://cck.iojbl.cn

C#:   Debug.Assert(x > 0);
来源：http://sau.guowangkeji.top

[H08] 获取错误信息与堆栈
来源：http://gut.bbcook.cn

Py:   str(e);  traceback.format_exc()
来源：http://zxp.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://itc.chenlongwang.top

JS:   e.message;  e.stack
来源：http://mic.birdmap.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qyi.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://olf.cashguo.top

Go:   err.Error()
来源：http://nkn.shanyushiyangtech.top

Ruby: e.message;  e.backtrace
来源：http://wcd.zhiwuduotai.top

C#:   e.Message;  e.StackTrace
来源：http://twh.quarkkingdee.top

[H09] 带错误码的异常
来源：http://tir.haohaochexian.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://szr.jyoumei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xjr.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://slp.wangshuangyany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ltx.shanyushiyangtech.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ffx.52xcode.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hiq.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tjq.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://vqr.bbcook.cn

[H10] 资源自动释放
来源：http://vzt.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://qpm.pengpengdd.cyou

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rtm.zhoulong.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bdi.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ssb.snrcjt.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cmc.svipenyu.cn

Go:   defer f.Close()
来源：http://rwh.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rwr.pycfn.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pqt.shangyingyoupin.top

================================================================================
来源：http://ehd.zycfv.cn

I. 正则表达式
来源：http://efh.cheryme.top

================================================================================
来源：http://wex.quarkkingdee.top

[I01] 判断是否匹配
来源：http://tnn.dianchejie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qvq.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://msf.yanxiufei.cn

JS:   /\d+/.test(s)
来源：http://fja.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://ugq.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mqy.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ffr.fengsongda.top

Ruby: s.match?(/\d+/)
来源：http://lsw.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bsq.fktsv.cn

[I02] 提取所有匹配
来源：http://vay.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://mub.nanxuanxn.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dnx.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://auu.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://tzi.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yav.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dkn.hammf.cn

Ruby: s.scan(/\d+/)
来源：http://ouv.tian-w.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nxo.dianchejie.cn

[I03] 提取捕获分组
来源：http://ure.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hqj.yangfankeji.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fiu.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vcz.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pjy.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://idn.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hpv.kuanghao11.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jom.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hpo.mhx1999.top

[I04] 正则替换
来源：http://ajn.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wlm.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gkk.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://qsq.tianlin.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://jtg.yuanzhike.top

Java: s.replaceAll("\\d+", "#")
来源：http://syx.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jzk.hammf.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hxa.tanke756.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jce.yonumen.top

[I05] 按正则拆分
来源：http://xap.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sum.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qgy.haohaochexian.top

JS:   s.split(/\s*,\s*/)
来源：http://fzt.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://obl.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://aqh.wangshuangyany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wpi.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://cjg.hnxiangtu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wzg.jinqigfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ufs.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vjo.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://anp.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://now.vehdjk.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sso.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qih.mhx1999.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://glu.ydzc1.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wlq.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tqt.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://jlw.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ikm.snrcjt.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gwk.zycfv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://scr.cashguo.top

TS:   /error/gim
来源：http://bzy.dashuyun.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://afn.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xzv.cqqwz.cn

Ruby: s.scan(/error/i)
来源：http://qyn.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zyd.shuidangran.top

[I08] 贪婪与非贪婪匹配
来源：http://smw.fengsongda.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://inu.c1oappe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://reo.jinghuilouyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cmg.ppjwa.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kfv.shanyushiyangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vjd.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fxy.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://chz.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wom.jinqigufen.top

================================================================================
来源：http://wlq.gaohongyu789.top

J. 日期与时间
来源：http://hwm.yfazqb.com

================================================================================
来源：http://bwx.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://iqa.yanxiufei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ubk.haohaochexian.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://arn.epnwcf.com

JS:   new Date();  Date.now()
来源：http://kfg.fzhhl.top

TS:   new Date();  Date.now()
来源：http://gqi.zhoulong.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://klc.ywan-chungtsiang.top

Go:   time.Now()
来源：http://zmx.wangdashe.top

Ruby: Time.now
来源：http://wzm.yuxming.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bwe.tianlin.xyz

[J02] 格式化输出
来源：http://kqx.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dnr.gaohongyu789.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vje.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yip.zhiwuduotai.top

TS:   d.toISOString()
来源：http://aap.vehdjk.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zpr.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nqn.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kym.jinyuanbaomall.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dvh.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://quv.tian-w.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://osl.gogol.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jmg.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://vng.jyoumei.cn

TS:   new Date("2024-01-02")
来源：http://dhi.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://dro.hfpthk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mpx.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://meo.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ift.gaohongyu789.top

[J04] 时间戳与日期互转
来源：http://ezs.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hgh.gotoacloud.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://okh.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dtc.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vus.vehdjk.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dbl.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tzx.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ozh.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tac.zdqjudy.top

[J05] 时间加减（加 7 天）
来源：http://kim.bbcook.cn

Py:   now + timedelta(days=7)
来源：http://moo.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://ldv.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ora.sxryk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ihn.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://cvc.yuanzhike.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://whi.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://vvn.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://hkf.yj20258888.top

[J06] 计算两时间之差
来源：http://kbx.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://tjm.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://dxu.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oct.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://grb.ybcxt.top

Java: Duration.between(start, end).toSeconds()
来源：http://kxs.yongpay.top

Go:   end.Sub(start).Hours()
来源：http://fnu.zycfv.cn

Ruby: end - start                 # 返回秒数
来源：http://lry.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://prz.zhixingplan.top

[J07] 比较两个日期
来源：http://aon.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://fyb.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pij.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cxv.nanxuanxn.top

TS:   d1.getTime() < d2.getTime()
来源：http://cdw.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wgw.quarkkingdee.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://owb.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://toa.uphjek.com

C#:   d1 < d2;  d1 == d2
来源：http://czg.xinyue.icu

[J08] 提取年月日与星期
来源：http://ocg.yonumen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://snk.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jgt.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fnn.zdqjudy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ltv.guannengcc.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fqd.ybcxt.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wku.xziqi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uil.yuxming.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qwy.ctjpmb.com

[J09] 时区处理
来源：http://eks.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ueq.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iyk.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gou.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cmr.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sce.pycfn.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zpl.svipenyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://crh.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ozs.hcnkem.com

[J10] 取今天 / 本月第一天
来源：http://icn.cashguo.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zid.yueranfly.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hcx.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aik.shangyingyoupin.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rtc.fehbvm.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fja.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vnt.9152youxi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mxh.zhijiandao.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pis.kuanghao11.cn

================================================================================
来源：http://hpk.jinghuilouyu.cn

K. JSON 与序列化
来源：http://nje.yanxiufei.cn

================================================================================
来源：http://tey.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://nxf.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uth.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ush.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://diw.havefunace.top

TS:   JSON.stringify(obj)
来源：http://agv.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fif.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://wny.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://pus.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://uhi.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://orq.xinyue.icu

Py:   json.loads(s)
来源：http://tiw.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mao.meibo888.top

JS:   JSON.parse(s)
来源：http://mfd.jianghu66.top

TS:   JSON.parse(s)
来源：http://pvm.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pbo.cashguo.top

Go:   json.Unmarshal(data, &v)
来源：http://ptr.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://buf.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://voq.zhoulong.xyz

[K03] JSON 美化输出（带缩进）
来源：http://mjt.0kj1m.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ctx.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fna.pengpengdd.cyou

JS:   JSON.stringify(obj, null, 2)
来源：http://lfy.xziqi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fqw.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://whn.dashuyun.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jti.hongshengwenyu.top

Ruby: JSON.pretty_generate(obj)
来源：http://ptr.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mwh.9152youxi.cn

[K04] 读取 JSON 文件
来源：http://wog.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jkm.xziqi.cn


<!-- 参考信息 -->