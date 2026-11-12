代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://nma.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mfs.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://fkt.yangfankeji.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nhh.iojbl.cn

PHP:  get_object_vars($obj);
来源：http://jvd.tian-w.cn

JS:   Object.entries(obj)
来源：http://gnn.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://jhm.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rni.ywan-chungtsiang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bnb.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://wiz.ehwqpu.com

C#:   // 用反射或 System.Text.Json
来源：http://mue.ybcxt.top

================================================================================
来源：http://erx.hfpthk.cn

H. 异常与错误处理
来源：http://csq.xuetiantiany.cn

================================================================================
来源：http://zhz.ppjwa.cn

[H01] try / catch 基础
来源：http://ver.zhiwuduotai.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eca.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zqm.xuanzx.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vav.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ffr.cqqwz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eea.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://get.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lsn.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jyl.fzhhl.top

[H02] finally / ensure 收尾
来源：http://ofc.fanxiaobao.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://mzz.dashuyun.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://prk.wangdashe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vck.pengpengdd.cyou

TS:   try { f(); } finally { cleanup(); }
来源：http://aco.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://itf.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ymd.52xcode.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://szg.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wmp.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://nom.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://meq.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://scr.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://mjy.316326.xyz

TS:   throw new Error("错误信息");
来源：http://hou.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rer.yfazqb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xbw.zhijiandao.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ial.jinyuanbaomall.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bqn.hysaishi.cn

[H04] 自定义异常类型
来源：http://evi.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://utp.guannengcc.top

PHP:  class MyError extends RuntimeException {}
来源：http://fwd.yonumen.top

JS:   class MyError extends Error {}
来源：http://mum.xylfe.cn

TS:   class MyError extends Error {}
来源：http://kur.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://iwe.chenzaomai.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jpc.vehdjk.com

Ruby: class MyError < StandardError; end
来源：http://beq.cheryme.top

C#:   class MyException : Exception {}
来源：http://mqd.xziqi.cn

[H05] 捕获特定类型
来源：http://jau.ehwqpu.com

Py:   except ValueError as e:
来源：http://vfs.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dxp.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://skr.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://rno.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://myb.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kyj.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://bep.c1oappe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://his.daxiang520.top

[H06] 可选值 / 空值安全访问
来源：http://wws.yueranfly.top

Py:   value = d.get("k") or default
来源：http://ury.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://oyo.zhengqikj.top

JS:   obj?.a?.b;  d ?? default
来源：http://gzx.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://moq.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ycf.nanxuanxn.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bsv.feifeiyinyue.top

Ruby: d&.dig(:a, :b)
来源：http://tft.shuidangran.top

C#:   obj?.A?.B ?? default
来源：http://pah.ehwqpu.com

[H07] 断言
来源：http://acm.birdmap.top

Py:   assert x > 0, "必须为正"
来源：http://eym.svipenyu.cn

PHP:  assert($x > 0);
来源：http://lxw.xuanzx.com

JS:   console.assert(x > 0);
来源：http://dcp.svipenyu.cn

TS:   console.assert(x > 0);
来源：http://wox.daxiang520.top

Java: assert x > 0 : "必须为正";
来源：http://gmk.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cwd.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://umk.ivvv.top

C#:   Debug.Assert(x > 0);
来源：http://oaf.redwolf501.top

[H08] 获取错误信息与堆栈
来源：http://pqe.uphjek.com

Py:   str(e);  traceback.format_exc()
来源：http://ljm.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fuc.epnwcf.com

JS:   e.message;  e.stack
来源：http://yfn.sjlbkw.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mbk.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://srk.pycfn.com

Go:   err.Error()
来源：http://ahl.xinyue.icu

Ruby: e.message;  e.backtrace
来源：http://qoc.nwbrower.top

C#:   e.Message;  e.StackTrace
来源：http://ugi.yangfankeji.com

[H09] 带错误码的异常
来源：http://fpp.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fuj.tianlin.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://asl.cucudq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xvg.daria6918.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ytk.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bgb.hnxiangtu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ccr.yfazqb.com

Ruby: raise MyError.new("fail", 500)
来源：http://kup.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hjc.cdnleiting.top

[H10] 资源自动释放
来源：http://blf.chenjidiqi.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://jwo.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ihb.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gkr.redwolf501.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fpp.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ptv.xingfuxueyuan.xyz

Go:   defer f.Close()
来源：http://kts.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eme.zhijiandao.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nlz.aibaodan.cn

================================================================================
来源：http://nzm.cucudq.cn

I. 正则表达式
来源：http://jit.hfpthk.cn

================================================================================
来源：http://zeg.sysykeji.top

[I01] 判断是否匹配
来源：http://jcz.yuxming.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rbr.fengsongda.top

PHP:  preg_match('/\d+/', $s);
来源：http://jnx.yj20258.top

JS:   /\d+/.test(s)
来源：http://efc.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://oag.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lqc.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oiq.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://ipt.zdbjq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rhf.vqdsnc.cn

[I02] 提取所有匹配
来源：http://yct.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://xpw.nanxinkj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://heh.dashuyun.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://far.chenlongwang.top

TS:   s.match(/\d+/g)
来源：http://jjq.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pcp.pycfn.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pzo.zhongyouzk.top

Ruby: s.scan(/\d+/)
来源：http://zux.pycfn.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pgt.bjfxy.top

[I03] 提取捕获分组
来源：http://ihx.uphjek.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gom.zhongyouzk.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nrc.jqgufenzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qhh.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gdi.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rni.zhijiandao.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mfk.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://owd.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fnj.cqqwz.cn

[I04] 正则替换
来源：http://ggh.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tji.nanxinkj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tsx.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://zhk.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nbs.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://ifh.52xcode.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yrq.hammf.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zoc.ivvv.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tcd.hcnkem.com

[I05] 按正则拆分
来源：http://xej.hongshengwenyu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bnk.hesvh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wiv.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://rdk.gogol.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://soa.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://shl.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ctr.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vay.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mgl.sjlbkw.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oxo.kuanghao11.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jia.guannengcc.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nei.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lnl.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://olk.yvedp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vxe.ywan-chungtsiang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kdh.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kdw.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ahi.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://fdk.yvedp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pzz.tanke756.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xaf.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ygn.xziqi.cn

TS:   /error/gim
来源：http://ugi.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tqr.jinghuilouyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jkc.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://fwj.sweek.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://isl.hywenlv.cn

[I08] 贪婪与非贪婪匹配
来源：http://pxy.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hux.hnxiangtu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jgy.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://leb.yangfankeji.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gbx.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jrn.guowangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ruw.guannengcc.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://osp.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sei.xylfe.cn

================================================================================
来源：http://txg.tanke756.top

J. 日期与时间
来源：http://lxo.ydzc1.top

================================================================================
来源：http://ive.andypj.xyz

[J01] 获取当前时间
来源：http://khr.haohaochexian.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mta.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mqj.sxryk.cn

JS:   new Date();  Date.now()
来源：http://ldk.ehwqpu.com

TS:   new Date();  Date.now()
来源：http://glt.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pcw.xylfe.cn

Go:   time.Now()
来源：http://fae.yj202588.top

Ruby: Time.now
来源：http://olf.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xfb.cashguo.top

[J02] 格式化输出
来源：http://aqm.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kvt.316326.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qhg.dashuyun.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pgg.zhongyouzk.top

TS:   d.toISOString()
来源：http://dvo.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lsg.hywenlv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bvn.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kly.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hlm.ivvv.top

[J03] 字符串解析为日期
来源：http://bgb.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rly.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mqu.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://pwa.yanxiufei.cn

TS:   new Date("2024-01-02")
来源：http://gqp.fktsv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gvi.fanxiaobao.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qda.meibo888.top

Ruby: Date.parse("2024-01-02")
来源：http://esi.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://int.haohaochexian.top

[J04] 时间戳与日期互转
来源：http://hnl.fengsongda.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://khf.jyoumei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zir.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://saj.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qqv.yuxming.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wyd.yj20258.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wru.zhengqikj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://drp.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rle.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://pev.zdbjq.cn

Py:   now + timedelta(days=7)
来源：http://eog.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ucs.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fof.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nsx.fzhhl.top

Java: LocalDate.now().plusDays(7)
来源：http://cac.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fiq.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://egc.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://bgs.yuxming.cn

[J06] 计算两时间之差
来源：http://qkf.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://ltp.smart0.xyz

PHP:  $end->diff($start)->days;
来源：http://vmc.svipenyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ahk.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wzj.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://hqf.wangdashe.top

Go:   end.Sub(start).Hours()
来源：http://xza.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://ezf.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://fvg.redwolf501.top

[J07] 比较两个日期
来源：http://lqd.ydzc1.top

Py:   d1 < d2;  d1 == d2
来源：http://oxx.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bqq.chenzaomai.com

JS:   d1.getTime() < d2.getTime()
来源：http://sum.hammf.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ryn.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tsq.gogol.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aol.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://hsj.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://ese.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://lig.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eji.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nko.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tuu.svipenyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xfb.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gjs.tarul.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dqt.tian-w.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yfp.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ftv.xziqi.cn

[J09] 时区处理
来源：http://gxe.jinqigufen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ffy.uphjek.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xws.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rig.nanxuanxn.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gwn.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cdj.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ohj.fzhhl.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pxq.ybcxt.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ewo.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://jfh.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qmx.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oal.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hzp.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zex.kuanghao11.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://znm.yuanzhike.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://auv.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rfc.tian-w.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kcz.bjfxy.top

================================================================================
来源：http://inc.daxiang520.top

K. JSON 与序列化
来源：http://thu.fengsongda.top

================================================================================
来源：http://sbk.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://wmn.haohaochexian.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gho.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uye.sjlbkw.cn

JS:   JSON.stringify(obj)
来源：http://pvj.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://ttl.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://huc.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://zfe.guannengcc.top

Ruby: obj.to_json                                     // require "json"
来源：http://mvr.yuxming.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qfy.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://xrz.havefunace.top

Py:   json.loads(s)
来源：http://hjy.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uai.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://exr.dianchejie.cn

TS:   JSON.parse(s)
来源：http://edk.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://swa.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://mir.yj20258888.top

Ruby: JSON.parse(s)
来源：http://xbb.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rng.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://pua.pycfn.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eyz.zdqjudy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sor.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yhx.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vux.nanxuanxn.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tlu.pycfn.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zwm.ivvv.top


<!-- 参考信息 -->