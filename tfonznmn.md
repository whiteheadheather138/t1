代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://lwr.shanyushiyangtech.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fvy.yj202588.top

[G16] 对象转数组 / 字典
来源：http://rkv.hongshengwenyu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rvs.birdmap.top

PHP:  get_object_vars($obj);
来源：http://lpw.sufxvd.cn

JS:   Object.entries(obj)
来源：http://jgm.cucudq.cn

TS:   Object.entries(obj)
来源：http://sms.jinqigfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jyx.vehdjk.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://clv.uphjek.com

Ruby: obj.instance_variables
来源：http://eme.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://qgg.yuanzhike.top

================================================================================
来源：http://brv.316326.xyz

H. 异常与错误处理
来源：http://src.yonumen.top

================================================================================
来源：http://ddo.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://fso.hywenlv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hez.wangdashe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hyx.ppjwa.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lfs.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nmk.jinqigfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hzi.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nen.yongpay.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vxd.yongpay.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pat.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://zjo.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://ule.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://eex.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ndu.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qhw.sxryk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cas.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vkl.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://iqo.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nzq.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://rju.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://wwa.jqgfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vid.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://tkm.svipenyu.cn

TS:   throw new Error("错误信息");
来源：http://cit.sweek.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kaf.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://acs.zhijiandao.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://njv.jiagoushi.top

C#:   throw new ArgumentException("错误信息");
来源：http://yto.quarkkingdee.top

[H04] 自定义异常类型
来源：http://ubo.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://wrr.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://djk.hysaishi.cn

JS:   class MyError extends Error {}
来源：http://vok.9152youxi.cn

TS:   class MyError extends Error {}
来源：http://rpv.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://hls.yanxiufei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ice.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://wqk.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://jzz.yfazqb.com

[H05] 捕获特定类型
来源：http://znr.nwbrower.top

Py:   except ValueError as e:
来源：http://alu.yangfankeji.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bbi.haohaochexian.top

JS:   if (e instanceof TypeError) {}
来源：http://vwe.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://lyn.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://xoo.pengpengdd.cyou

Go:   errors.Is(err, os.ErrNotExist)
来源：http://miz.ydzc1.top

Ruby: rescue ArgumentError => e
来源：http://nan.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sib.ppjwa.cn

[H06] 可选值 / 空值安全访问
来源：http://gyi.hnqzz.top

Py:   value = d.get("k") or default
来源：http://fix.andypj.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://hyj.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://lnr.sysykeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://gfk.hammf.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pfp.cdnleiting.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hcn.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://wtn.jlsjyb.cn

C#:   obj?.A?.B ?? default
来源：http://hvc.daria6918.cn

[H07] 断言
来源：http://nfe.bbcook.cn

Py:   assert x > 0, "必须为正"
来源：http://rwk.yvedp.cn

PHP:  assert($x > 0);
来源：http://bfp.yonumen.top

JS:   console.assert(x > 0);
来源：http://ubu.fengsongda.top

TS:   console.assert(x > 0);
来源：http://tyz.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://yfd.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eff.xylfe.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jdr.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://yuj.ybcxt.top

[H08] 获取错误信息与堆栈
来源：http://dff.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://svb.yfazqb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lur.yj20258.top

JS:   e.message;  e.stack
来源：http://cmc.vehdjk.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://jlu.ybcxt.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cdh.xingfuxueyuan.xyz

Go:   err.Error()
来源：http://nzo.c1oappe.top

Ruby: e.message;  e.backtrace
来源：http://qyo.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://ypz.chenlongwang.top

[H09] 带错误码的异常
来源：http://jea.cdnleiting.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qny.9152youxi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wpt.feifeiyinyue.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://teo.zycfv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qez.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dyb.dashuyun.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rdl.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://dcq.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rph.iojbl.cn

[H10] 资源自动释放
来源：http://gkd.fzhhl.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://crp.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wyk.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fjy.yj20258888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://htf.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://med.jinqigfzy.top

Go:   defer f.Close()
来源：http://gxv.yonumen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kkn.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ckf.sxryk.cn

================================================================================
来源：http://uot.hcnkem.com

I. 正则表达式
来源：http://rpo.yongpay.top

================================================================================
来源：http://umh.yuxming.cn

[I01] 判断是否匹配
来源：http://btf.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wuy.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://odq.jianghu66.top

JS:   /\d+/.test(s)
来源：http://cyh.ywan-chungtsiang.top

TS:   /\d+/.test(s)
来源：http://yao.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fmy.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://njv.fehbvm.com

Ruby: s.match?(/\d+/)
来源：http://xpg.sweek.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ebm.xziqi.cn

[I02] 提取所有匹配
来源：http://fxc.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://knr.ybcxt.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ikl.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zsz.fktsv.cn

TS:   s.match(/\d+/g)
来源：http://nem.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tab.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jnd.epnwcf.com

Ruby: s.scan(/\d+/)
来源：http://meu.jqgfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jbd.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://uvf.jqgufenzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nda.dashuyun.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wjy.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pbu.zhiwuduotai.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qvi.jinqigufen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cfr.havefunace.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mue.yj20258888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://txq.xuanzx.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hhh.zdqjudy.top

[I04] 正则替换
来源：http://juj.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ypd.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vwc.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://lfk.daria6918.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sty.fzhhl.top

Java: s.replaceAll("\\d+", "#")
来源：http://pon.yonumen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xti.birdmap.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xdc.ivvv.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jzc.zhijiandao.cn

[I05] 按正则拆分
来源：http://hqo.zhaomingkeji.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://vhk.316326.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eak.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://riy.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://fov.hywenlv.cn

Java: s.split("\\s*,\\s*")
来源：http://wmn.chenzaomai.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nqa.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://isn.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rie.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ibf.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ijg.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://stu.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cpj.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fkn.yongpay.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rkj.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mac.iojbl.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://paz.aibaodan.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wmj.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://wuu.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kyc.andypj.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://crh.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qfe.hongshengwenyu.top

TS:   /error/gim
来源：http://rrn.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hqa.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qbo.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://zde.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ysf.aibaodan.cn

[I08] 贪婪与非贪婪匹配
来源：http://cqg.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dho.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iiq.gaohongyu789.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ell.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rqn.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://enh.yanxiufei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vgs.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ofd.hnqzz.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wux.bbcook.cn

================================================================================
来源：http://pui.sxryk.cn

J. 日期与时间
来源：http://din.ivvv.top

================================================================================
来源：http://hoy.zycfv.cn

[J01] 获取当前时间
来源：http://utd.hfpthk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wki.tanke756.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lfb.xuanzx.com

JS:   new Date();  Date.now()
来源：http://hyj.yonumen.top

TS:   new Date();  Date.now()
来源：http://xbl.gaohongyu789.top

Java: LocalDateTime.now();  Instant.now()
来源：http://teh.jinqigfzy.top

Go:   time.Now()
来源：http://aoi.shzxlz.cn

Ruby: Time.now
来源：http://ekd.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dms.epnwcf.com

[J02] 格式化输出
来源：http://mcc.0kj1m.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tpy.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gkp.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mql.ybcxt.top

TS:   d.toISOString()
来源：http://plg.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uex.cucudq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hfn.jinqigfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ago.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ltk.ydzc1.top

[J03] 字符串解析为日期
来源：http://yrk.xinyue.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bnl.hongshengwenyu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uyu.ctjpmb.com

JS:   new Date("2024-01-02")
来源：http://vkq.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://gob.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://elr.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gmh.sysykeji.top

Ruby: Date.parse("2024-01-02")
来源：http://okv.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cfz.ydzc1.top

[J04] 时间戳与日期互转
来源：http://wre.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vha.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qmu.smart0.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uma.nanxinkj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yqs.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hwj.gzhubu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cbb.yj20258888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lni.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sep.nanxuanxn.top

[J05] 时间加减（加 7 天）
来源：http://wcy.fanxiaobao.xyz

Py:   now + timedelta(days=7)
来源：http://ptd.yangfankeji.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://nby.hfpthk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://exo.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cjo.zhongyouzk.top

Java: LocalDate.now().plusDays(7)
来源：http://rch.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xfb.wangdashe.top

Ruby: Time.now + 7 * 86400
来源：http://ygd.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://csb.bjfxy.top

[J06] 计算两时间之差
来源：http://pee.hnxiangtu.top

Py:   (end - start).total_seconds()
来源：http://zcb.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://deq.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://esb.gotoacloud.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://alv.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mbm.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://doa.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://vxt.shanyushiyangtech.top

C#:   (end - start).TotalSeconds
来源：http://tft.fengsongda.top

[J07] 比较两个日期
来源：http://bmi.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://isj.dianchejie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eai.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://jcl.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://epv.fehbvm.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nxv.yvedp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vsq.wangshuangyany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ype.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://kmd.cdnleiting.top

[J08] 提取年月日与星期
来源：http://hed.fengsongda.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uoz.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sam.shzxlz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dcc.aizwys.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kle.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cgh.smart0.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zhe.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xnb.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mlj.wangdashe.top

[J09] 时区处理
来源：http://rxw.jinqigufen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zcx.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jud.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eoj.c1oappe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zyb.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qbl.yuxming.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tgm.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jfp.jiagoushi.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lbl.zhiwuduotai.top

[J10] 取今天 / 本月第一天
来源：http://gfm.yangfankeji.com

Py:   date.today();  date.today().replace(day=1)
来源：http://igq.tanke756.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ema.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zcb.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nhm.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wqw.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jiv.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://weu.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wve.wangshuangyany.cn

================================================================================
来源：http://vzk.ydjk.org.cn

K. JSON 与序列化
来源：http://ydc.kuanghao11.cn

================================================================================
来源：http://hgp.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://bip.jqgufenzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://icn.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lpu.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://mcf.hammf.cn

TS:   JSON.stringify(obj)
来源：http://jui.fanxiaobao.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cgz.daria6918.cn

Go:   json.Marshal(obj)
来源：http://vnq.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://acq.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lwd.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://exh.cashguo.top

Py:   json.loads(s)
来源：http://sdh.tianlin.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xkj.hfpthk.cn

JS:   JSON.parse(s)
来源：http://keb.jyoumei.cn

TS:   JSON.parse(s)
来源：http://dtx.jinqigfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://umg.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://thp.sxryk.cn

Ruby: JSON.parse(s)
来源：http://aab.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://feb.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://mej.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://psm.ehwqpu.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rhc.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xfw.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://iam.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mzo.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ess.tanke756.top


<!-- 参考信息 -->