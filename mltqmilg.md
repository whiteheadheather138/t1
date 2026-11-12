代发 wailian999

PHP:  get_object_vars($obj);
来源：http://xnb.bjfxy.top

JS:   Object.entries(obj)
来源：http://mko.zdbjq.cn

TS:   Object.entries(obj)
来源：http://zvv.jyoumei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vpk.shuidangran.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sbg.svipenyu.cn

Ruby: obj.instance_variables
来源：http://dqf.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://rcj.havefunace.top

================================================================================
来源：http://csq.guannengcc.top

H. 异常与错误处理
来源：http://fzt.yj202588.top

================================================================================
来源：http://xyg.yfazqb.com

[H01] try / catch 基础
来源：http://mlz.bbcook.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ynm.snrcjt.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fku.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ait.yj202588.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://esz.bjfxy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zwa.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dgp.jinyuanbaomall.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://awf.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fwn.uphjek.com

[H02] finally / ensure 收尾
来源：http://vlz.svipenyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tco.tian-w.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fiy.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ioq.zhengqikj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bxk.zhengqikj.top

Java: try { f(); } finally { cleanup(); }
来源：http://aqr.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nln.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wnd.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://inq.gaohongyu789.top

[H03] 主动抛出异常
来源：http://mul.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://twi.316326.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xgg.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://rfd.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://kuc.kuanghao11.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://igy.hnqzz.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://agw.zhijiandao.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ybk.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uzd.fanxiaobao.xyz

[H04] 自定义异常类型
来源：http://rqe.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://czh.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://rqe.zhaomingkeji.xyz

JS:   class MyError extends Error {}
来源：http://ujn.nwbrower.top

TS:   class MyError extends Error {}
来源：http://zgs.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://fij.zycfv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cqn.0kj1m.cn

Ruby: class MyError < StandardError; end
来源：http://rzf.iojbl.cn

C#:   class MyException : Exception {}
来源：http://djn.aizwys.cn

[H05] 捕获特定类型
来源：http://unv.wangdashe.top

Py:   except ValueError as e:
来源：http://vgg.yj20258.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ehy.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://pyh.birdmap.top

TS:   if (e instanceof TypeError) {}
来源：http://jzh.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://woe.yvedp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ntj.wangdashe.top

Ruby: rescue ArgumentError => e
来源：http://nkr.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zun.meibo888.top

[H06] 可选值 / 空值安全访问
来源：http://vzx.fzhhl.top

Py:   value = d.get("k") or default
来源：http://ihh.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://xhh.meibo888.top

JS:   obj?.a?.b;  d ?? default
来源：http://ufx.jianghu66.top

TS:   obj?.a?.b;  d ?? default
来源：http://liq.hfpthk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://szz.yanxiufei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rtl.yuanzhike.top

Ruby: d&.dig(:a, :b)
来源：http://drq.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://gfm.fanxiaobao.xyz

[H07] 断言
来源：http://skb.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://ycd.pengpengdd.cyou

PHP:  assert($x > 0);
来源：http://ctx.epnwcf.com

JS:   console.assert(x > 0);
来源：http://dvy.yongpay.top

TS:   console.assert(x > 0);
来源：http://uuj.chenzaomai.com

Java: assert x > 0 : "必须为正";
来源：http://vwu.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xap.birdmap.top

Ruby: raise "必须为正" unless x > 0
来源：http://kwn.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://sqb.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://emq.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://qqu.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bqd.nwbrower.top

JS:   e.message;  e.stack
来源：http://ecp.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://qvx.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://afa.sysykeji.top

Go:   err.Error()
来源：http://foq.tian-w.cn

Ruby: e.message;  e.backtrace
来源：http://mlw.xinyue.icu

C#:   e.Message;  e.StackTrace
来源：http://uup.gaohongyu789.top

[H09] 带错误码的异常
来源：http://ggy.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://icf.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pnm.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://srx.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://twj.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rub.yangfankeji.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://txl.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://esb.jyoumei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://msl.ehwqpu.com

[H10] 资源自动释放
来源：http://qjn.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://obw.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gmk.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oyr.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kfm.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tlp.yj20258.top

Go:   defer f.Close()
来源：http://ium.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aew.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ipy.xziqi.cn

================================================================================
来源：http://unb.sysykeji.top

I. 正则表达式
来源：http://nun.yfazqb.com

================================================================================
来源：http://lpc.daxiang520.top

[I01] 判断是否匹配
来源：http://nus.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hcg.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nux.fengsongda.top

JS:   /\d+/.test(s)
来源：http://cqi.xylfe.cn

TS:   /\d+/.test(s)
来源：http://can.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vly.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://abp.cqqwz.cn

Ruby: s.match?(/\d+/)
来源：http://nym.fktsv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ppn.ydjk.org.cn

[I02] 提取所有匹配
来源：http://iav.dianchejie.cn

Py:   re.findall(r"\d+", s)
来源：http://irs.zhongyouzk.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fgh.zhixingplan.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://skl.cashguo.top

TS:   s.match(/\d+/g)
来源：http://vlx.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dgl.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tcq.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://nkd.smart0.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fvh.jiagoushi.top

[I03] 提取捕获分组
来源：http://rav.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tpi.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://khm.xinyue.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iix.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://noe.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qxe.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rxz.ivvv.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fvi.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wzj.tarul.cn

[I04] 正则替换
来源：http://nec.hfpthk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sbu.hysaishi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rjw.xingfuxueyuan.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://gqc.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://njr.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yqv.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://qxs.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ykt.hfpthk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ifl.ydzc1.top

[I05] 按正则拆分
来源：http://mne.sjlbkw.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hwr.dianchejie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pxd.nanxuanxn.top

JS:   s.split(/\s*,\s*/)
来源：http://lnk.svipenyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://ypy.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://fhg.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ixa.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://jly.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zbg.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://siu.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tif.wangshuangyany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://liw.daxiang520.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pby.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qqd.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://omn.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://apz.cqqwz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://twy.yfazqb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uki.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://tzv.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://whd.birdmap.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qdd.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ntz.ctjpmb.com

TS:   /error/gim
来源：http://bcv.fktsv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hek.ivvv.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ttu.daria6918.cn

Ruby: s.scan(/error/i)
来源：http://pyq.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nzv.c1oappe.top

[I08] 贪婪与非贪婪匹配
来源：http://vxq.meibo888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://okc.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hrg.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bgd.yanxiufei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qdv.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sur.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rnp.wangshuangyany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gdc.quarkkingdee.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pdp.xziqi.cn

================================================================================
来源：http://jaf.haohaochexian.top

J. 日期与时间
来源：http://sld.uphjek.com

================================================================================
来源：http://vea.yuanzhike.top

[J01] 获取当前时间
来源：http://rwn.ivvv.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://znc.jqgfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hqc.guowangkeji.top

JS:   new Date();  Date.now()
来源：http://jpm.yj20258.top

TS:   new Date();  Date.now()
来源：http://zss.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zjl.wangdashe.top

Go:   time.Now()
来源：http://tyi.zdbjq.cn

Ruby: Time.now
来源：http://cpn.xylfe.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://plh.ybcxt.top

[J02] 格式化输出
来源：http://ced.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ddi.sysykeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uuw.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hgh.wangdashe.top

TS:   d.toISOString()
来源：http://bza.cashguo.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cub.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://inp.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://icl.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zyl.havefunace.top

[J03] 字符串解析为日期
来源：http://een.aibaodan.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dpf.hcnkem.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xrm.zycfv.cn

JS:   new Date("2024-01-02")
来源：http://xmn.bjfxy.top

TS:   new Date("2024-01-02")
来源：http://jdk.xylfe.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nmb.hongshengwenyu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bnm.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://yzj.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pzc.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://api.yueranfly.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hru.sjlbkw.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zsa.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jfp.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://phl.tanke756.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ujr.pengpengdd.cyou

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bbz.xylfe.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kls.jlsjyb.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kxo.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://had.jinqigufen.top

Py:   now + timedelta(days=7)
来源：http://ctt.tianlin.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://xrp.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ziv.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vab.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://cqs.zhaomingkeji.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pdu.hfpthk.cn

Ruby: Time.now + 7 * 86400
来源：http://gwt.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://pco.tian-w.cn

[J06] 计算两时间之差
来源：http://mjh.chenzaomai.com

Py:   (end - start).total_seconds()
来源：http://bth.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://ang.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qdl.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qiv.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://vcj.smart0.xyz

Go:   end.Sub(start).Hours()
来源：http://drf.wangdashe.top

Ruby: end - start                 # 返回秒数
来源：http://dhe.shanyushiyangtech.top

C#:   (end - start).TotalSeconds
来源：http://ldo.nanxuanxn.top

[J07] 比较两个日期
来源：http://qyx.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://swv.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lij.sufxvd.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xlh.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://nih.jinqigufen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fbc.jinyuanbaomall.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://het.fanxiaobao.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://tgu.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://wza.snrcjt.cn

[J08] 提取年月日与星期
来源：http://lbk.guannengcc.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ixb.chenlongwang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uwn.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ueh.dashuyun.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fdd.redwolf501.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ddz.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sya.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://adb.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hhm.daria6918.cn

[J09] 时区处理
来源：http://yxd.zhiwuduotai.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hlm.nanxinkj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lhj.yfazqb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yrf.yonumen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mru.daria6918.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vzf.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nom.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tys.uphjek.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aiw.jinyuanbaomall.cn

[J10] 取今天 / 本月第一天
来源：http://tpd.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://esg.aizwys.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ssr.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iny.hcnkem.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sbb.zhijiandao.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://irf.ydzc1.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://awy.pycfn.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cft.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sby.feifeiyinyue.top

================================================================================
来源：http://vav.jqgfzy.top

K. JSON 与序列化
来源：http://zod.gotoacloud.top

================================================================================
来源：http://tzi.bbcook.cn

[K01] 对象转 JSON 字符串
来源：http://ixg.xuanzx.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uwv.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://luh.zhoulong.xyz

JS:   JSON.stringify(obj)
来源：http://dfp.sweek.top

TS:   JSON.stringify(obj)
来源：http://zhg.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pvp.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://jrw.zycfv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ooy.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://idf.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://zco.yfazqb.com

Py:   json.loads(s)
来源：http://hzq.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sbl.yueranfly.top

JS:   JSON.parse(s)
来源：http://ojk.sweek.top

TS:   JSON.parse(s)
来源：http://agz.sufxvd.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mks.tian-w.cn

Go:   json.Unmarshal(data, &v)
来源：http://hzy.yuxming.cn

Ruby: JSON.parse(s)
来源：http://apy.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zfm.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://sdv.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tya.jianghu66.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dre.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qmy.haohaochexian.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jfh.zhengqikj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vub.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wko.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://udm.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mkq.jqgfzy.top

[K04] 读取 JSON 文件
来源：http://eab.ppjwa.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://erl.0kj1m.cn


<!-- 参考信息 -->