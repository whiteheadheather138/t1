代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://otb.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kpz.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://dtj.wangdashe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bws.yonumen.top

PHP:  get_object_vars($obj);
来源：http://lge.yfazqb.com

JS:   Object.entries(obj)
来源：http://kap.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://fbo.hesvh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tgw.shangyingyoupin.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cpa.yangfankeji.com

Ruby: obj.instance_variables
来源：http://sni.zhongyouzk.top

C#:   // 用反射或 System.Text.Json
来源：http://tfh.pycfn.com

================================================================================
来源：http://yfd.sufxvd.cn

H. 异常与错误处理
来源：http://uwk.yongpay.top

================================================================================
来源：http://gdw.jqgufenzy.top

[H01] try / catch 基础
来源：http://upm.dashuyun.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lzv.jinqigufen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cmr.aibaodan.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aag.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ojx.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cgw.birdmap.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fty.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jhv.zhongyouzk.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rhe.guowangkeji.top

[H02] finally / ensure 收尾
来源：http://onl.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://bxi.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lwk.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hwp.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vnz.zycfv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xsy.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hem.pycfn.com

Ruby: begin; f; ensure; cleanup; end
来源：http://asv.tian-w.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bgv.zhijiandao.cn

[H03] 主动抛出异常
来源：http://onk.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://vhc.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pnn.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://qtv.dashuyun.cn

TS:   throw new Error("错误信息");
来源：http://qxw.zhoulong.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://ihi.yvedp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vkf.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ags.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dhv.zhengqikj.top

[H04] 自定义异常类型
来源：http://zen.yj202588.top

Py:   class MyError(Exception): pass
来源：http://yym.pycfn.com

PHP:  class MyError extends RuntimeException {}
来源：http://vrc.dashuyun.cn

JS:   class MyError extends Error {}
来源：http://ftw.316326.xyz

TS:   class MyError extends Error {}
来源：http://dpi.havefunace.top

Java: class MyException extends RuntimeException {}
来源：http://aed.jinqigfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jax.sjlbkw.cn

Ruby: class MyError < StandardError; end
来源：http://lbp.fktsv.cn

C#:   class MyException : Exception {}
来源：http://aey.dianchejie.cn

[H05] 捕获特定类型
来源：http://dco.fanxiaobao.xyz

Py:   except ValueError as e:
来源：http://hfb.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zcx.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://ifc.gaohongyu789.top

TS:   if (e instanceof TypeError) {}
来源：http://fyu.kuanghao11.cn

Java: catch (IOException | SQLException e) {}
来源：http://znj.tianlin.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gad.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://gnn.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lbm.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://ftf.bjfxy.top

Py:   value = d.get("k") or default
来源：http://kvu.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://akc.gzhubu.top

JS:   obj?.a?.b;  d ?? default
来源：http://ghm.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://jsn.jiagoushi.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lky.xinyue.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://wnf.fktsv.cn

Ruby: d&.dig(:a, :b)
来源：http://det.yonumen.top

C#:   obj?.A?.B ?? default
来源：http://mdh.ydjk.org.cn

[H07] 断言
来源：http://tqc.bjfxy.top

Py:   assert x > 0, "必须为正"
来源：http://phb.shanyushiyangtech.top

PHP:  assert($x > 0);
来源：http://dhg.yfazqb.com

JS:   console.assert(x > 0);
来源：http://nnd.vehdjk.com

TS:   console.assert(x > 0);
来源：http://ukm.sufxvd.cn

Java: assert x > 0 : "必须为正";
来源：http://qay.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dha.gaohongyu789.top

Ruby: raise "必须为正" unless x > 0
来源：http://lvf.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://vdo.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://uie.bjfxy.top

Py:   str(e);  traceback.format_exc()
来源：http://vpy.yvedp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vvu.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://uax.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://iwi.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ihr.52xcode.cn

Go:   err.Error()
来源：http://acf.sysykeji.top

Ruby: e.message;  e.backtrace
来源：http://pju.yongpay.top

C#:   e.Message;  e.StackTrace
来源：http://xlo.zhixingplan.top

[H09] 带错误码的异常
来源：http://atn.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vlc.shanyushiyangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://oss.ctjpmb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hiw.zhengqikj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://avn.wangshuangyany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mjw.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://avg.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hnl.hongshengwenyu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nbj.shuidangran.top

[H10] 资源自动释放
来源：http://emb.jqgfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mpq.fktsv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dnn.ywan-chungtsiang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://olt.tarul.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ldq.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pbv.zdbjq.cn

Go:   defer f.Close()
来源：http://nbf.xylfe.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wat.fzhhl.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://afx.jyoumei.cn

================================================================================
来源：http://xac.xinyue.icu

I. 正则表达式
来源：http://adk.daria6918.cn

================================================================================
来源：http://jqa.zhongyouzk.top

[I01] 判断是否匹配
来源：http://zdw.jianghu66.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gzy.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://wop.hcnkem.com

JS:   /\d+/.test(s)
来源：http://vej.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://yhp.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uzx.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wmh.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://fyf.hysaishi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nse.meibo888.top

[I02] 提取所有匹配
来源：http://cwg.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://xzn.wangshuangyany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://how.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xnl.havefunace.top

TS:   s.match(/\d+/g)
来源：http://qza.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dqh.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vos.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://zph.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dkh.hnqzz.top

[I03] 提取捕获分组
来源：http://soj.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wwm.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nrk.jinyuanbaomall.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cmm.cheryme.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fic.snrcjt.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tkm.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qwx.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dke.jianghu66.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cbt.hnxiangtu.top

[I04] 正则替换
来源：http://ejv.sweek.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zxg.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bjz.zhoulong.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://bqf.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://cga.shangyingyoupin.top

Java: s.replaceAll("\\d+", "#")
来源：http://wrs.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yxi.hongshengwenyu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hpd.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lpv.ydjk.org.cn

[I05] 按正则拆分
来源：http://eep.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://xmh.hysaishi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lfs.yuanzhike.top

JS:   s.split(/\s*,\s*/)
来源：http://kgh.gaohongyu789.top

TS:   s.split(/\s*,\s*/)
来源：http://onq.ctjpmb.com

Java: s.split("\\s*,\\s*")
来源：http://fap.aibaodan.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fdo.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://qbc.yj20258888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fyx.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ynp.nwbrower.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xog.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sqe.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oqb.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bxa.zhoulong.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bdn.zhixingplan.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zrr.bbcook.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sfw.gaohongyu789.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ses.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://bhl.xuetiantiany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://coy.wangdashe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iox.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://owk.hongshengwenyu.top

TS:   /error/gim
来源：http://zbh.sxryk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://frg.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sou.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://tri.fzhhl.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rdc.jlsjyb.cn

[I08] 贪婪与非贪婪匹配
来源：http://pcc.feifeiyinyue.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tnq.daria6918.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lnq.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gsl.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bfx.shuidangran.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mtq.jiagoushi.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mzw.feifeiyinyue.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gqp.jinqigufen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gah.hesvh.cn

================================================================================
来源：http://aom.guannengcc.top

J. 日期与时间
来源：http://uvu.yvedp.cn

================================================================================
来源：http://jee.yueranfly.top

[J01] 获取当前时间
来源：http://cel.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kzp.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pvv.yonumen.top

JS:   new Date();  Date.now()
来源：http://npo.jinghuilouyu.cn

TS:   new Date();  Date.now()
来源：http://ejk.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qdc.9152youxi.cn

Go:   time.Now()
来源：http://ntw.xylfe.cn

Ruby: Time.now
来源：http://luq.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://piw.shzxlz.cn

[J02] 格式化输出
来源：http://stq.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://acu.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wzb.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bcf.tanke756.top

TS:   d.toISOString()
来源：http://fwt.shzxlz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aee.sufxvd.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vjo.sweek.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sgk.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zed.sysykeji.top

[J03] 字符串解析为日期
来源：http://eaq.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cnu.iojbl.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://grr.dashuyun.cn

JS:   new Date("2024-01-02")
来源：http://qhg.ywan-chungtsiang.top

TS:   new Date("2024-01-02")
来源：http://ebl.andypj.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://gfh.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dae.9152youxi.cn

Ruby: Date.parse("2024-01-02")
来源：http://chk.ywan-chungtsiang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qbf.gzhubu.top

[J04] 时间戳与日期互转
来源：http://jrz.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xug.cucudq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ovb.yueranfly.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jld.xylfe.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jeo.jinyuanbaomall.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gqp.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://koy.smart0.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qty.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ygm.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://fpw.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://hmo.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ebc.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hgh.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hxj.jinqigfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://oxs.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qbd.jqgufenzy.top

Ruby: Time.now + 7 * 86400
来源：http://tda.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://zoj.mhx1999.top

[J06] 计算两时间之差
来源：http://ewm.gzhubu.top

Py:   (end - start).total_seconds()
来源：http://nze.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://qui.gzhubu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bpe.ybcxt.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rsw.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://djt.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://zrm.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://yiy.chenzaomai.com

C#:   (end - start).TotalSeconds
来源：http://ond.jlsjyb.cn

[J07] 比较两个日期
来源：http://dkc.hongshengwenyu.top

Py:   d1 < d2;  d1 == d2
来源：http://qfu.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rgy.yanxiufei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mcj.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://rks.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jsp.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://axi.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://ryc.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://ifg.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://oyd.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://att.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://msi.iojbl.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qio.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://suv.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fnv.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zaf.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wbd.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xkg.xylfe.cn

[J09] 时区处理
来源：http://bgl.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tqo.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tek.yvedp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hwk.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dke.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ige.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yhj.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nav.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ubx.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://nlr.jinqigufen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wik.cucudq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ftt.shanyushiyangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hiz.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wrk.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zqu.jinyuanbaomall.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yep.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mmm.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bsg.jlsjyb.cn

================================================================================
来源：http://zqi.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://nef.nanxuanxn.top

================================================================================
来源：http://ufb.vehdjk.com

[K01] 对象转 JSON 字符串
来源：http://pai.gotoacloud.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://krk.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oen.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://yxz.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://yqp.cucudq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cpi.xingfuxueyuan.xyz

Go:   json.Marshal(obj)
来源：http://ujw.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zxm.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yhg.c1oappe.top

[K02] JSON 字符串转对象
来源：http://hie.chenlongwang.top

Py:   json.loads(s)
来源：http://rar.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ydl.tanke756.top

JS:   JSON.parse(s)
来源：http://ngg.dashuyun.cn

TS:   JSON.parse(s)
来源：http://ndm.zhixingplan.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qgg.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://zzo.zhengqikj.top

Ruby: JSON.parse(s)
来源：http://ita.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lnd.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://hyg.zhengqikj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qln.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kpe.shanyushiyangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xty.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://vcu.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ktv.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ynv.wangdashe.top


<!-- 参考信息 -->