代发 wailian999

H. 异常与错误处理
来源：http://giu.xuetiantiany.cn

================================================================================
来源：http://zba.gogol.net.cn

[H01] try / catch 基础
来源：http://deb.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jyp.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fol.daxiang520.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://end.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ewn.52xcode.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vra.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://khf.dashuyun.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://azr.jinqigfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wyn.uphjek.com

[H02] finally / ensure 收尾
来源：http://dxc.vqdsnc.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bdv.shangyingyoupin.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gew.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://eec.hongshengwenyu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yak.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zll.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lar.hfpthk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mwr.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://cwj.mhx1999.top

[H03] 主动抛出异常
来源：http://nfu.smart0.xyz

Py:   raise ValueError("错误信息")
来源：http://rbe.smart0.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ghq.epnwcf.com

JS:   throw new Error("错误信息");
来源：http://eko.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://oxb.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nbt.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ymh.yj20258.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zhi.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://and.snrcjt.cn

[H04] 自定义异常类型
来源：http://gvd.jinyuanbaomall.cn

Py:   class MyError(Exception): pass
来源：http://zbm.ivvv.top

PHP:  class MyError extends RuntimeException {}
来源：http://obw.yfazqb.com

JS:   class MyError extends Error {}
来源：http://jzr.tanke756.top

TS:   class MyError extends Error {}
来源：http://eja.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://fsg.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kvx.chenzaomai.com

Ruby: class MyError < StandardError; end
来源：http://zaz.chenjidiqi.icu

C#:   class MyException : Exception {}
来源：http://meh.vqdsnc.cn

[H05] 捕获特定类型
来源：http://xfh.meibo888.top

Py:   except ValueError as e:
来源：http://jqd.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pvf.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://rrz.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://zlk.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://anm.tianlin.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dtq.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://doz.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://azt.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://jau.fanxiaobao.xyz

Py:   value = d.get("k") or default
来源：http://pba.nanxuanxn.top

PHP:  $v = $d["k"] ?? null;
来源：http://njj.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://use.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://vfo.chenjidiqi.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lnr.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wze.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://tnd.zhiwuduotai.top

C#:   obj?.A?.B ?? default
来源：http://hxa.sufxvd.cn

[H07] 断言
来源：http://the.bjfxy.top

Py:   assert x > 0, "必须为正"
来源：http://nvv.hfpthk.cn

PHP:  assert($x > 0);
来源：http://qaq.vehdjk.com

JS:   console.assert(x > 0);
来源：http://grt.tarul.cn

TS:   console.assert(x > 0);
来源：http://niu.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://snq.jinyuanbaomall.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nrn.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ffg.ydzc1.top

C#:   Debug.Assert(x > 0);
来源：http://auv.shzxlz.cn

[H08] 获取错误信息与堆栈
来源：http://tfh.0kj1m.cn

Py:   str(e);  traceback.format_exc()
来源：http://xik.andypj.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tmp.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://zxp.hywenlv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uuw.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qdr.feifeiyinyue.top

Go:   err.Error()
来源：http://hzj.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://hxi.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://kdt.bjfxy.top

[H09] 带错误码的异常
来源：http://cot.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fme.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://imn.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gxo.guowangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yzj.redwolf501.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iwc.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cbu.tarul.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kli.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xtb.pengpengdd.cyou

[H10] 资源自动释放
来源：http://kzp.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://zun.xinyue.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kqn.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mok.9152youxi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zcq.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mps.jyoumei.cn

Go:   defer f.Close()
来源：http://eow.cdnleiting.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xuu.yongpay.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lly.jinqigfzy.top

================================================================================
来源：http://aqw.quarkkingdee.top

I. 正则表达式
来源：http://hxj.aizwys.cn

================================================================================
来源：http://zke.jinqigfzy.top

[I01] 判断是否匹配
来源：http://xdw.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xky.sxryk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://orl.hywenlv.cn

JS:   /\d+/.test(s)
来源：http://yup.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://nnc.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://url.xuanzx.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ujr.hcnkem.com

Ruby: s.match?(/\d+/)
来源：http://opm.dianchejie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wct.daxiang520.top

[I02] 提取所有匹配
来源：http://ecw.jianghu66.top

Py:   re.findall(r"\d+", s)
来源：http://yen.zhongyouzk.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qec.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lzy.kuanghao11.cn

TS:   s.match(/\d+/g)
来源：http://alk.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pxd.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cdd.cashguo.top

Ruby: s.scan(/\d+/)
来源：http://zxw.hysaishi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eta.sysykeji.top

[I03] 提取捕获分组
来源：http://wbz.zdqjudy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lzo.yvedp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dea.nanxinkj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hox.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vhx.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rah.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fxu.tianlin.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ome.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://spu.jqgufenzy.top

[I04] 正则替换
来源：http://oup.yonumen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://eza.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tzt.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://puy.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jfe.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://cns.xuetiantiany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yle.fehbvm.com

Ruby: s.gsub(/\d+/, "#")
来源：http://bde.shuidangran.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vhs.nwbrower.top

[I05] 按正则拆分
来源：http://wif.ywan-chungtsiang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wfo.shanyushiyangtech.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rqs.guannengcc.top

JS:   s.split(/\s*,\s*/)
来源：http://tjl.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://cdq.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://jal.xuetiantiany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rtl.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mam.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ili.gaohongyu789.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://epe.cucudq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yot.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xvt.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pmz.tanke756.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fba.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rzz.fanxiaobao.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vmn.andypj.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fbr.yvedp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hmc.zhongyouzk.top

[I07] 忽略大小写与多行模式
来源：http://uvp.shangyingyoupin.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bvt.yonumen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sel.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dji.nanxinkj.top

TS:   /error/gim
来源：http://phz.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://htq.yj20258.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://glv.ctjpmb.com

Ruby: s.scan(/error/i)
来源：http://lwk.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://awn.guowangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://xct.hywenlv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xrb.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://izn.ybcxt.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://otv.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dlz.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zqc.ybcxt.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xpc.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nbz.zdbjq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vjx.xylfe.cn

================================================================================
来源：http://ikb.ivvv.top

J. 日期与时间
来源：http://ren.quarkkingdee.top

================================================================================
来源：http://llu.dianchejie.cn

[J01] 获取当前时间
来源：http://gov.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ech.cdnleiting.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yai.hnqzz.top

JS:   new Date();  Date.now()
来源：http://nla.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://gfs.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tni.hywenlv.cn

Go:   time.Now()
来源：http://ecy.snrcjt.cn

Ruby: Time.now
来源：http://hwj.sysykeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gii.aizwys.cn

[J02] 格式化输出
来源：http://msb.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dat.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jac.xingfuxueyuan.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lpt.quarkkingdee.top

TS:   d.toISOString()
来源：http://moa.smart0.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gmn.zhoulong.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zjm.yj202588.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zlf.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fml.epnwcf.com

[J03] 字符串解析为日期
来源：http://gyj.fzhhl.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xpq.xuetiantiany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sfu.hnqzz.top

JS:   new Date("2024-01-02")
来源：http://nnq.quarkkingdee.top

TS:   new Date("2024-01-02")
来源：http://ezw.pycfn.com

Java: LocalDate.parse("2024-01-02")
来源：http://sbk.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kgm.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://rnf.shzxlz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://goj.birdmap.top

[J04] 时间戳与日期互转
来源：http://uii.jqgfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tbn.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uyv.svipenyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vzr.guannengcc.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nxk.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://noa.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gtk.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xzx.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cge.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://njo.andypj.xyz

Py:   now + timedelta(days=7)
来源：http://gvu.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dfd.ydjk.org.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bdg.yanxiufei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://skp.nwbrower.top

Java: LocalDate.now().plusDays(7)
来源：http://qut.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mmy.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://bjh.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://eai.bjfxy.top

[J06] 计算两时间之差
来源：http://uxq.yj202588.top

Py:   (end - start).total_seconds()
来源：http://rak.nwbrower.top

PHP:  $end->diff($start)->days;
来源：http://ehw.hfpthk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vhi.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fld.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://krt.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://jnw.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://xle.sweek.top

C#:   (end - start).TotalSeconds
来源：http://brt.yj202588.top

[J07] 比较两个日期
来源：http://idb.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://pof.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://onl.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://evu.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://rwr.cashguo.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hfh.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ngl.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://bzf.shanyushiyangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://fny.cheryme.top

[J08] 提取年月日与星期
来源：http://eqd.daxiang520.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ddr.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fxm.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://btg.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vgn.xuetiantiany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kzn.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yfb.ppjwa.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cdz.xingfuxueyuan.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pca.hysaishi.cn

[J09] 时区处理
来源：http://ctw.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fxe.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://clg.tian-w.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jwg.zhiwuduotai.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://smt.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lop.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sic.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://crb.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fcp.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://ill.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ejg.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://otr.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ymj.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mbk.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yvq.birdmap.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dod.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uof.gotoacloud.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mpd.9152youxi.cn

================================================================================
来源：http://tqk.hesvh.cn

K. JSON 与序列化
来源：http://owy.ywan-chungtsiang.top

================================================================================
来源：http://qcu.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://sol.yj20258888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://owp.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fbp.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://deu.316326.xyz

TS:   JSON.stringify(obj)
来源：http://fcg.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pwf.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://uap.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://tkb.smart0.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://xpf.hnqzz.top

[K02] JSON 字符串转对象
来源：http://miq.zycfv.cn

Py:   json.loads(s)
来源：http://xmi.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ema.smart0.xyz

JS:   JSON.parse(s)
来源：http://ovu.316326.xyz

TS:   JSON.parse(s)
来源：http://yln.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rhl.ehwqpu.com

Go:   json.Unmarshal(data, &v)
来源：http://hri.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://hmn.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tun.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://ngn.tian-w.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pdv.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vnc.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oqu.hnqzz.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ipt.52xcode.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dqa.52xcode.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sck.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://xhu.nanxinkj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zyw.hcnkem.com

[K04] 读取 JSON 文件
来源：http://wch.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ogz.chenlongwang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hvx.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dmd.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://big.dianchejie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tof.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wkv.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mec.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jru.tarul.cn

[K05] 深拷贝对象
来源：http://rkn.vqdsnc.cn


<!-- 参考信息 -->