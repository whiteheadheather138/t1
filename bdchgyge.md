代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://ehy.zdbjq.cn

Ruby: obj.instance_variables
来源：http://qsv.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://ghn.fengsongda.top

================================================================================
来源：http://wke.yonumen.top

H. 异常与错误处理
来源：http://qiy.guannengcc.top

================================================================================
来源：http://qry.xuanzx.com

[H01] try / catch 基础
来源：http://apy.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lny.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lzp.mhx1999.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oyn.jyoumei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ked.zhengqikj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rnl.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zdu.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mqc.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xet.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://vws.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://sps.yangfankeji.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://yav.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zgm.kuanghao11.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tyh.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ung.fktsv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kzx.xinyue.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://fkv.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://snc.ehwqpu.com

[H03] 主动抛出异常
来源：http://nic.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://lec.jiagoushi.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yta.jlsjyb.cn

JS:   throw new Error("错误信息");
来源：http://rsd.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://emy.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pan.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zjr.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wab.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://xlu.hammf.cn

[H04] 自定义异常类型
来源：http://tfq.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://uoe.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qad.wangshuangyany.cn

JS:   class MyError extends Error {}
来源：http://oxx.yj202588.top

TS:   class MyError extends Error {}
来源：http://wbt.sysykeji.top

Java: class MyException extends RuntimeException {}
来源：http://rkm.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mtb.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://swl.xylfe.cn

C#:   class MyException : Exception {}
来源：http://mky.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://equ.bjfxy.top

Py:   except ValueError as e:
来源：http://ryr.nanxuanxn.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fiy.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://tqe.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://oln.chenzaomai.com

Java: catch (IOException | SQLException e) {}
来源：http://fyc.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lzn.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://wzy.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wjx.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://ymt.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://tsl.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://ohg.zhixingplan.top

JS:   obj?.a?.b;  d ?? default
来源：http://bzo.zhongyouzk.top

TS:   obj?.a?.b;  d ?? default
来源：http://rti.ppjwa.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cwx.hcnkem.com

Go:   if v, ok := m["k"]; ok { }
来源：http://gvx.ydjk.org.cn

Ruby: d&.dig(:a, :b)
来源：http://npe.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://exl.yvedp.cn

[H07] 断言
来源：http://suy.316326.xyz

Py:   assert x > 0, "必须为正"
来源：http://nsi.hywenlv.cn

PHP:  assert($x > 0);
来源：http://ugz.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://cce.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://gbr.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://wek.yvedp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bfm.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://eop.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://vez.yueranfly.top

[H08] 获取错误信息与堆栈
来源：http://hzb.dashuyun.cn

Py:   str(e);  traceback.format_exc()
来源：http://cap.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://khk.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://uar.iojbl.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rja.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://zsy.yangfankeji.com

Go:   err.Error()
来源：http://bei.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://hdg.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://gam.guannengcc.top

[H09] 带错误码的异常
来源：http://xbc.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://doy.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://tdi.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://agz.haohaochexian.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rjf.bjfxy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zxr.quarkkingdee.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://msb.meibo888.top

Ruby: raise MyError.new("fail", 500)
来源：http://btu.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oam.xuanzx.com

[H10] 资源自动释放
来源：http://dxr.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ygi.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zoa.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nwm.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eyh.sufxvd.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cad.zhongyouzk.top

Go:   defer f.Close()
来源：http://vxz.sufxvd.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wlq.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://luy.haohaochexian.top

================================================================================
来源：http://qkk.ivvv.top

I. 正则表达式
来源：http://ndx.pengpengdd.cyou

================================================================================
来源：http://kdt.havefunace.top

[I01] 判断是否匹配
来源：http://mip.bbcook.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nqo.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://wqb.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://ims.shanyushiyangkeji.top

TS:   /\d+/.test(s)
来源：http://niz.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yrg.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ilh.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://vha.cashguo.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cbv.jlsjyb.cn

[I02] 提取所有匹配
来源：http://oiu.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://gvo.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pzc.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ahw.xuetiantiany.cn

TS:   s.match(/\d+/g)
来源：http://fux.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://suo.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fdn.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://wlp.yangfankeji.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tet.cqqwz.cn

[I03] 提取捕获分组
来源：http://qgi.cashguo.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://isd.cqqwz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gks.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ibp.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://urj.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nia.jqgufenzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zkl.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nzj.shangyingyoupin.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iqu.gaohongyu789.top

[I04] 正则替换
来源：http://ixb.guowangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sri.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://azz.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://qzd.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fdm.jqgfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://gny.shzxlz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://glz.svipenyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uxc.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fqt.zhixingplan.top

[I05] 按正则拆分
来源：http://xhf.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://cqs.aibaodan.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dio.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://czx.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://ldw.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://wcz.zhongyouzk.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jvd.hesvh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wio.yonumen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ffj.xylfe.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ugx.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yql.yangfankeji.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dhb.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://msw.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pmv.xylfe.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zjj.haohaochexian.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://poh.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nqo.yueranfly.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iwn.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://uio.yj202588.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sek.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gbk.jlsjyb.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://izj.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://sqq.hnqzz.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://seo.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fkm.ydzc1.top

Ruby: s.scan(/error/i)
来源：http://eip.shuidangran.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://azf.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://qrj.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zxk.ehwqpu.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zfx.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ybx.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ict.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://psa.jinqigufen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oxd.fktsv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qcy.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zlj.fengsongda.top

================================================================================
来源：http://xuo.dianchejie.cn

J. 日期与时间
来源：http://hup.pycfn.com

================================================================================
来源：http://duo.hfpthk.cn

[J01] 获取当前时间
来源：http://hjw.cheryme.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://trz.xylfe.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wnm.gaohongyu789.top

JS:   new Date();  Date.now()
来源：http://cvc.quarkkingdee.top

TS:   new Date();  Date.now()
来源：http://wsq.ivvv.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nnn.daxiang520.top

Go:   time.Now()
来源：http://ppi.vehdjk.com

Ruby: Time.now
来源：http://tzy.jqgufenzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fah.hcnkem.com

[J02] 格式化输出
来源：http://dag.gaohongyu789.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qrm.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fyv.hammf.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kgs.cucudq.cn

TS:   d.toISOString()
来源：http://uvg.hnxiangtu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zvk.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://skd.kuanghao11.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://syx.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vmm.haohaochexian.top

[J03] 字符串解析为日期
来源：http://wjq.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mxt.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nec.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://vnn.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://iyd.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://vbq.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://apy.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://xss.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dzi.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://khe.dashuyun.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://brw.cucudq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jza.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mvl.316326.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://klr.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zvg.mhx1999.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://axd.sufxvd.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dzr.sufxvd.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zyi.ydzc1.top

[J05] 时间加减（加 7 天）
来源：http://vux.sweek.top

Py:   now + timedelta(days=7)
来源：http://fil.c1oappe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gdv.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yja.xuanzx.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qtg.yongpay.top

Java: LocalDate.now().plusDays(7)
来源：http://xvt.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wcp.hcnkem.com

Ruby: Time.now + 7 * 86400
来源：http://adc.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://hei.ydjk.org.cn

[J06] 计算两时间之差
来源：http://zfb.snrcjt.cn

Py:   (end - start).total_seconds()
来源：http://jqg.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://mwb.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ozc.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sxk.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jgf.sjlbkw.cn

Go:   end.Sub(start).Hours()
来源：http://lbt.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://qsd.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://hqb.wangdashe.top

[J07] 比较两个日期
来源：http://zhj.sxryk.cn

Py:   d1 < d2;  d1 == d2
来源：http://bum.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yxa.hysaishi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gyb.xingfuxueyuan.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://hvl.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wvh.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dfu.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://gee.ehwqpu.com

C#:   d1 < d2;  d1 == d2
来源：http://nft.chenzaomai.com

[J08] 提取年月日与星期
来源：http://mso.cdnleiting.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://msf.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ikf.iojbl.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zuj.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lms.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mpi.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kiu.uphjek.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hpk.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lve.bjfxy.top

[J09] 时区处理
来源：http://gcx.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hkm.zdbjq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jjj.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vin.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jdz.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://exm.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hfs.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rtu.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qcc.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://iry.birdmap.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mft.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ywo.svipenyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xji.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://quf.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aet.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kjl.gaohongyu789.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pfq.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://foa.yj20258.top

================================================================================
来源：http://rcl.gogol.net.cn

K. JSON 与序列化
来源：http://amy.yj20258.top

================================================================================
来源：http://rpc.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://ore.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ncg.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vmr.hongshengwenyu.top

JS:   JSON.stringify(obj)
来源：http://vec.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://chl.meibo888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://szh.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://pqr.52xcode.cn

Ruby: obj.to_json                                     // require "json"
来源：http://apk.jqgfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ypl.yj20258888.top

[K02] JSON 字符串转对象
来源：http://kpy.jinqigufen.top

Py:   json.loads(s)
来源：http://exw.yongpay.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pid.yangfankeji.com

JS:   JSON.parse(s)
来源：http://agx.yuxming.cn

TS:   JSON.parse(s)
来源：http://uzg.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mkc.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://vgz.shanyushiyangkeji.top

Ruby: JSON.parse(s)
来源：http://shf.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mfq.bjfxy.top

[K03] JSON 美化输出（带缩进）
来源：http://fpv.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pkb.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ymn.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lam.ywan-chungtsiang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://oxc.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fqw.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hzu.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://nqa.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ccy.hysaishi.cn

[K04] 读取 JSON 文件
来源：http://qxf.hywenlv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ays.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vrt.ydzc1.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qma.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tno.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qjt.mhx1999.top


<!-- 参考信息 -->