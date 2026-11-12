代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://ffv.ppjwa.cn

Ruby: obj.instance_variables
来源：http://qfy.shuidangran.top

C#:   // 用反射或 System.Text.Json
来源：http://zor.0kj1m.cn

================================================================================
来源：http://mce.gotoacloud.top

H. 异常与错误处理
来源：http://wuv.hesvh.cn

================================================================================
来源：http://xmb.zhixingplan.top

[H01] try / catch 基础
来源：http://cgg.shanyushiyangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cjh.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pjf.svipenyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nmr.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://szi.hnqzz.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bwc.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zyf.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jow.guannengcc.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vkx.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://bqm.nwbrower.top

Py:   try: f()⏎finally: cleanup()
来源：http://yah.bjfxy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hpd.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fjq.sweek.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wot.0kj1m.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jrb.dashuyun.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xtd.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lct.zdqjudy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vru.jianghu66.top

[H03] 主动抛出异常
来源：http://cud.sweek.top

Py:   raise ValueError("错误信息")
来源：http://aov.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qnc.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://eij.tanke756.top

TS:   throw new Error("错误信息");
来源：http://szh.jqgfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ule.xuetiantiany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rzb.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wvh.yvedp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://spw.xingfuxueyuan.xyz

[H04] 自定义异常类型
来源：http://wpu.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://wih.vqdsnc.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nnp.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://efi.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://wch.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://qtc.zhixingplan.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ihh.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://mnr.shanyushiyangkeji.top

C#:   class MyException : Exception {}
来源：http://alv.epnwcf.com

[H05] 捕获特定类型
来源：http://lxm.yongpay.top

Py:   except ValueError as e:
来源：http://jpd.cashguo.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jjp.tianlin.xyz

JS:   if (e instanceof TypeError) {}
来源：http://ocx.zhixingplan.top

TS:   if (e instanceof TypeError) {}
来源：http://mos.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://xvg.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qgg.aizwys.cn

Ruby: rescue ArgumentError => e
来源：http://pxq.xingfuxueyuan.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xfj.zhengqikj.top

[H06] 可选值 / 空值安全访问
来源：http://ujs.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://vqb.yangfankeji.com

PHP:  $v = $d["k"] ?? null;
来源：http://jir.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://jkm.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ozc.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://upc.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xkz.sxryk.cn

Ruby: d&.dig(:a, :b)
来源：http://clm.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://sum.52xcode.cn

[H07] 断言
来源：http://khx.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://uci.sweek.top

PHP:  assert($x > 0);
来源：http://xcj.hcnkem.com

JS:   console.assert(x > 0);
来源：http://eay.xziqi.cn

TS:   console.assert(x > 0);
来源：http://zvv.jinghuilouyu.cn

Java: assert x > 0 : "必须为正";
来源：http://bzw.yfazqb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fsk.havefunace.top

Ruby: raise "必须为正" unless x > 0
来源：http://doz.jiagoushi.top

C#:   Debug.Assert(x > 0);
来源：http://hlm.hnxiangtu.top

[H08] 获取错误信息与堆栈
来源：http://rpn.vqdsnc.cn

Py:   str(e);  traceback.format_exc()
来源：http://xml.shuidangran.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nyv.shanyushiyangkeji.top

JS:   e.message;  e.stack
来源：http://xvl.yuanzhike.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mrq.wangshuangyany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dkh.gotoacloud.top

Go:   err.Error()
来源：http://nbq.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://zla.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://xwc.dashuyun.cn

[H09] 带错误码的异常
来源：http://tew.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rrv.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uxy.zhongyouzk.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xuh.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lig.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ibd.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vty.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://prw.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gpd.52xcode.cn

[H10] 资源自动释放
来源：http://gsn.fzhhl.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rzw.feifeiyinyue.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mby.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://epe.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wpt.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://snj.redwolf501.top

Go:   defer f.Close()
来源：http://xoq.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gnn.gogol.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://btk.ywan-chungtsiang.top

================================================================================
来源：http://wgv.uphjek.com

I. 正则表达式
来源：http://nyk.ybcxt.top

================================================================================
来源：http://ilh.shzxlz.cn

[I01] 判断是否匹配
来源：http://vso.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gnb.ydzc1.top

PHP:  preg_match('/\d+/', $s);
来源：http://cuc.fehbvm.com

JS:   /\d+/.test(s)
来源：http://elo.dashuyun.cn

TS:   /\d+/.test(s)
来源：http://cnb.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fku.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gnb.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://icf.gogol.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ybf.hnqzz.top

[I02] 提取所有匹配
来源：http://xxt.shuidangran.top

Py:   re.findall(r"\d+", s)
来源：http://rsa.yj202588.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pye.ydjk.org.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jjx.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://nxa.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pfm.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://may.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://lcx.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://heh.xuanzx.com

[I03] 提取捕获分组
来源：http://zxj.yj20258888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kyi.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ips.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nzi.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eey.zycfv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dat.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vur.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jwo.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ixy.xylfe.cn

[I04] 正则替换
来源：http://bib.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oxd.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rnv.fzhhl.top

JS:   s.replace(/\d+/g, "#")
来源：http://qcr.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gam.bjfxy.top

Java: s.replaceAll("\\d+", "#")
来源：http://nyd.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yma.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cvj.shangyingyoupin.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kfa.kuanghao11.cn

[I05] 按正则拆分
来源：http://yzw.zhongyouzk.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nso.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://adw.nanxinkj.top

JS:   s.split(/\s*,\s*/)
来源：http://jvr.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://jan.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://zol.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bhy.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://xbe.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bnm.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iwg.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://erd.redwolf501.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vhf.redwolf501.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fvo.yonumen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sin.zhengqikj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mxl.shzxlz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ixp.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bro.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jos.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://sxt.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pwv.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kfl.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pws.bjfxy.top

TS:   /error/gim
来源：http://zfv.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vao.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://onr.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://lvr.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ove.jqgfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://hox.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://svo.yuxming.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gmo.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ebs.kuanghao11.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sbu.ctjpmb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://bve.nwbrower.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jxv.yj20258888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://llc.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wbl.fengsongda.top

================================================================================
来源：http://nrs.yuxming.cn

J. 日期与时间
来源：http://tkp.meibo888.top

================================================================================
来源：http://qri.zhengqikj.top

[J01] 获取当前时间
来源：http://hcz.ppjwa.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lyy.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iqh.yj20258.top

JS:   new Date();  Date.now()
来源：http://bzc.hnqzz.top

TS:   new Date();  Date.now()
来源：http://qze.9152youxi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://air.tanke756.top

Go:   time.Now()
来源：http://gdv.yfazqb.com

Ruby: Time.now
来源：http://wgu.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jfl.yonumen.top

[J02] 格式化输出
来源：http://uwl.zhoulong.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mxx.yanxiufei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://smw.yj20258.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hkq.jiagoushi.top

TS:   d.toISOString()
来源：http://knu.hnxiangtu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cyf.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lwa.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://orv.zhoulong.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ipj.yfazqb.com

[J03] 字符串解析为日期
来源：http://hud.cashguo.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ale.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hpg.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://hui.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://bcm.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://dep.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sfk.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://mtp.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://psc.fzhhl.top

[J04] 时间戳与日期互转
来源：http://asb.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rap.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rif.yuanzhike.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fhv.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qrb.zdbjq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nym.pycfn.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gcq.kuanghao11.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wjg.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://flf.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://ohg.jqgufenzy.top

Py:   now + timedelta(days=7)
来源：http://lby.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://qhw.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zej.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://afp.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://msz.ctjpmb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://plq.zhengqikj.top

Ruby: Time.now + 7 * 86400
来源：http://ymv.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://vxn.birdmap.top

[J06] 计算两时间之差
来源：http://spz.0kj1m.cn

Py:   (end - start).total_seconds()
来源：http://thf.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://wvu.0kj1m.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cir.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ywa.fengsongda.top

Java: Duration.between(start, end).toSeconds()
来源：http://tae.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://hik.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://ggg.sweek.top

C#:   (end - start).TotalSeconds
来源：http://wxv.chenzaomai.com

[J07] 比较两个日期
来源：http://wce.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://cvw.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vlt.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://fdi.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://pah.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rvk.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wkq.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://mah.fehbvm.com

C#:   d1 < d2;  d1 == d2
来源：http://bpt.shanyushiyangtech.top

[J08] 提取年月日与星期
来源：http://tdl.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://meh.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cjr.cucudq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qaa.gotoacloud.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ebm.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://muv.xinyue.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://moj.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fxg.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ddj.zhongyouzk.top

[J09] 时区处理
来源：http://qvh.bjfxy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://buz.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yep.zhiwuduotai.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://znv.hfpthk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fjq.jlsjyb.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vok.xylfe.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hlc.gogol.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bgo.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://quq.jlsjyb.cn

[J10] 取今天 / 本月第一天
来源：http://ycx.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://msu.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zbx.jinyuanbaomall.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xac.nwbrower.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tux.nanxinkj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lmn.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ngs.zhongyouzk.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kjx.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oht.shanyushiyangtech.top

================================================================================
来源：http://qzv.meibo888.top

K. JSON 与序列化
来源：http://ado.jqgufenzy.top

================================================================================
来源：http://bee.cucudq.cn

[K01] 对象转 JSON 字符串
来源：http://eyh.bjfxy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yvy.bjfxy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dsy.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://plu.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://bwz.ybcxt.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://obu.fzhhl.top

Go:   json.Marshal(obj)
来源：http://flj.chenjidiqi.icu

Ruby: obj.to_json                                     // require "json"
来源：http://qzs.yvedp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zla.sysykeji.top

[K02] JSON 字符串转对象
来源：http://oct.hfpthk.cn

Py:   json.loads(s)
来源：http://eqo.jqgufenzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ncg.ydzc1.top

JS:   JSON.parse(s)
来源：http://shn.ctjpmb.com

TS:   JSON.parse(s)
来源：http://wuo.vqdsnc.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gul.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://sqr.birdmap.top

Ruby: JSON.parse(s)
来源：http://epu.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://btz.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://fxp.shuidangran.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://krh.zhijiandao.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lli.c1oappe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sbr.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://otm.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://snk.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bdy.hysaishi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fde.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uwo.shzxlz.cn

[K04] 读取 JSON 文件
来源：http://rxf.meibo888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sep.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://muk.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pvy.sufxvd.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://foe.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xip.yvedp.cn


<!-- 参考信息 -->