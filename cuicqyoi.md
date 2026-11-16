代发 wailian999

C#:   record User(string Name, int Age);
来源：http://atr.cashguo.top

[G15] 枚举
来源：http://qpq.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oqy.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gva.9152youxi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tru.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mlw.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://lyj.shangyingyoupin.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rim.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://mcy.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xhw.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://fis.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://upr.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://xfg.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://anc.redwolf501.top

TS:   Object.entries(obj)
来源：http://bwn.havefunace.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://arx.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cma.hysaishi.cn

Ruby: obj.instance_variables
来源：http://iih.nanxinkj.top

C#:   // 用反射或 System.Text.Json
来源：http://rbs.hcnkem.com

================================================================================
来源：http://hys.sweek.top

H. 异常与错误处理
来源：http://oii.tanke756.top

================================================================================
来源：http://wfl.cashguo.top

[H01] try / catch 基础
来源：http://wip.kuanghao11.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xmp.ybcxt.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xgl.sysykeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hod.hcnkem.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://utz.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rmt.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pot.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wky.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bds.hfpthk.cn

[H02] finally / ensure 收尾
来源：http://qhl.feifeiyinyue.top

Py:   try: f()⏎finally: cleanup()
来源：http://quq.jiagoushi.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yap.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ecr.tanke756.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kop.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://ckd.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bkl.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fiz.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dbx.jianghu66.top

[H03] 主动抛出异常
来源：http://uhr.gaohongyu789.top

Py:   raise ValueError("错误信息")
来源：http://xvh.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jcu.zhoulong.xyz

JS:   throw new Error("错误信息");
来源：http://hzd.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://sox.guowangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://you.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ktz.kuanghao11.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hyp.0kj1m.cn

C#:   throw new ArgumentException("错误信息");
来源：http://shq.fengsongda.top

[H04] 自定义异常类型
来源：http://htt.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://vbf.fzhhl.top

PHP:  class MyError extends RuntimeException {}
来源：http://tqo.nwbrower.top

JS:   class MyError extends Error {}
来源：http://dom.ppjwa.cn

TS:   class MyError extends Error {}
来源：http://pff.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://vvh.ywan-chungtsiang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ack.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://snv.yj20258888.top

C#:   class MyException : Exception {}
来源：http://qpz.yongpay.top

[H05] 捕获特定类型
来源：http://gfk.birdmap.top

Py:   except ValueError as e:
来源：http://iyq.cheryme.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tvd.zhaomingkeji.xyz

JS:   if (e instanceof TypeError) {}
来源：http://hhr.yj20258.top

TS:   if (e instanceof TypeError) {}
来源：http://ovw.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://cea.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zmj.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://kyl.zdbjq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eru.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://etd.iojbl.cn

Py:   value = d.get("k") or default
来源：http://mzj.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://pac.vqdsnc.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oox.ctjpmb.com

TS:   obj?.a?.b;  d ?? default
来源：http://mlx.yonumen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://esv.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://maq.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://acx.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://rkp.hammf.cn

[H07] 断言
来源：http://ehy.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://yvk.xuetiantiany.cn

PHP:  assert($x > 0);
来源：http://nbu.jqgfzy.top

JS:   console.assert(x > 0);
来源：http://loz.tarul.cn

TS:   console.assert(x > 0);
来源：http://xyr.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://yyb.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xoc.zhengqikj.top

Ruby: raise "必须为正" unless x > 0
来源：http://dol.ydzc1.top

C#:   Debug.Assert(x > 0);
来源：http://ttc.jinqigufen.top

[H08] 获取错误信息与堆栈
来源：http://ung.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://nix.zhoulong.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ggl.zhixingplan.top

JS:   e.message;  e.stack
来源：http://twc.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wjo.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://kyf.snrcjt.cn

Go:   err.Error()
来源：http://koi.yangfankeji.com

Ruby: e.message;  e.backtrace
来源：http://hdg.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://qus.sxryk.cn

[H09] 带错误码的异常
来源：http://ipj.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cwk.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://pio.shuidangran.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://egh.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ouy.tianlin.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pxe.ivvv.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ihk.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yru.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wpw.yueranfly.top

[H10] 资源自动释放
来源：http://jpc.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qhn.gotoacloud.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xkx.yuxming.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://byo.zdbjq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://imt.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://urb.nwbrower.top

Go:   defer f.Close()
来源：http://hqr.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gpt.yvedp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://izq.quarkkingdee.top

================================================================================
来源：http://ccp.yvedp.cn

I. 正则表达式
来源：http://aui.hammf.cn

================================================================================
来源：http://yln.shanyushiyangkeji.top

[I01] 判断是否匹配
来源：http://eiv.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://snh.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://loi.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://pfh.tanke756.top

TS:   /\d+/.test(s)
来源：http://oyc.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zan.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nki.ivvv.top

Ruby: s.match?(/\d+/)
来源：http://elt.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oql.wangshuangyany.cn

[I02] 提取所有匹配
来源：http://ikg.hywenlv.cn

Py:   re.findall(r"\d+", s)
来源：http://ali.pengpengdd.cyou

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ipx.jyoumei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kmt.vehdjk.com

TS:   s.match(/\d+/g)
来源：http://nxj.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lbv.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lis.yj20258888.top

Ruby: s.scan(/\d+/)
来源：http://ica.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jpu.jianghu66.top

[I03] 提取捕获分组
来源：http://udh.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ffq.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cni.cucudq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gwh.zhiwuduotai.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dql.zhongyouzk.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oes.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yab.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://czq.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hqj.guowangkeji.top

[I04] 正则替换
来源：http://wen.sxryk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ira.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ypb.zhoulong.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://yde.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://zhz.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://aas.uphjek.com

Go:   re.ReplaceAllString(s, "#")
来源：http://jmy.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uln.redwolf501.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qap.dianchejie.cn

[I05] 按正则拆分
来源：http://umf.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hsw.sufxvd.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rgu.jqgfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://fkt.jqgfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://ofv.chenzaomai.com

Java: s.split("\\s*,\\s*")
来源：http://yde.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jrm.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ody.jyoumei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yac.nanxuanxn.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hzp.jinyuanbaomall.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rsn.hnxiangtu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ujj.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mlk.svipenyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xvd.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fmx.fzhhl.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qcr.ybcxt.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ppd.sxryk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gcj.yj20258888.top

[I07] 忽略大小写与多行模式
来源：http://fjv.xuetiantiany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jed.316326.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ckk.zhixingplan.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kuj.bjfxy.top

TS:   /error/gim
来源：http://gyy.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ccp.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cxz.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://jnv.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gwl.hesvh.cn

[I08] 贪婪与非贪婪匹配
来源：http://psl.tarul.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ydq.jianghu66.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vuq.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://btv.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jca.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kzy.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ebv.hcnkem.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lsq.vqdsnc.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ruc.shanyushiyangtech.top

================================================================================
来源：http://rmu.zdbjq.cn

J. 日期与时间
来源：http://vtv.tarul.cn

================================================================================
来源：http://cgm.0kj1m.cn

[J01] 获取当前时间
来源：http://qrf.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://uxd.redwolf501.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pgo.ctjpmb.com

JS:   new Date();  Date.now()
来源：http://psv.ivvv.top

TS:   new Date();  Date.now()
来源：http://mqk.tarul.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zff.ydjk.org.cn

Go:   time.Now()
来源：http://ytn.ctjpmb.com

Ruby: Time.now
来源：http://oyt.wangdashe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sdv.fktsv.cn

[J02] 格式化输出
来源：http://ooq.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jfv.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://upd.fengsongda.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rin.c1oappe.top

TS:   d.toISOString()
来源：http://vhj.ivvv.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mzs.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oad.zhaomingkeji.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bmw.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tsh.hesvh.cn

[J03] 字符串解析为日期
来源：http://lkg.jqgufenzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aha.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mwt.guannengcc.top

JS:   new Date("2024-01-02")
来源：http://jeg.ivvv.top

TS:   new Date("2024-01-02")
来源：http://zaj.ydjk.org.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xwp.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ivy.bbcook.cn

Ruby: Date.parse("2024-01-02")
来源：http://acr.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jew.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://agr.fanxiaobao.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gwn.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jsz.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mee.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://pny.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wmd.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://euh.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nys.xingfuxueyuan.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wbn.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://zlc.cdnleiting.top

Py:   now + timedelta(days=7)
来源：http://kvo.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://lwj.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aev.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kzs.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://pci.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lwd.tian-w.cn

Ruby: Time.now + 7 * 86400
来源：http://wpg.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://mme.cucudq.cn

[J06] 计算两时间之差
来源：http://yyi.quarkkingdee.top

Py:   (end - start).total_seconds()
来源：http://ybf.hcnkem.com

PHP:  $end->diff($start)->days;
来源：http://oik.zhongyouzk.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nus.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://atg.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zqg.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://xif.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://rdi.ivvv.top

C#:   (end - start).TotalSeconds
来源：http://gnf.tian-w.cn

[J07] 比较两个日期
来源：http://sfs.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://lne.316326.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hru.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://rdb.fzhhl.top

TS:   d1.getTime() < d2.getTime()
来源：http://uka.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cjr.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://loo.chenjidiqi.icu

Ruby: d1 < d2;  d1 == d2
来源：http://jca.gzhubu.top

C#:   d1 < d2;  d1 == d2
来源：http://lve.hysaishi.cn

[J08] 提取年月日与星期
来源：http://net.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bui.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rtk.haohaochexian.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qxy.bjfxy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tof.nwbrower.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vjh.jinyuanbaomall.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://swl.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jiz.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lyx.jianghu66.top

[J09] 时区处理
来源：http://apl.xylfe.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://efe.kuanghao11.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hbn.fehbvm.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yil.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ggp.hcnkem.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oat.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mii.zycfv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uct.tarul.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://olb.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://fpd.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mdr.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jfa.zhixingplan.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vyi.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://syo.daria6918.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iqv.gzhubu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lqd.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cex.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gzm.yuxming.cn

================================================================================
来源：http://boy.zdqjudy.top

K. JSON 与序列化
来源：http://dcj.fehbvm.com

================================================================================
来源：http://bez.hfpthk.cn

[K01] 对象转 JSON 字符串
来源：http://otn.cheryme.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://atb.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ver.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://hji.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://ahk.ydzc1.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qwi.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://vjx.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wth.nwbrower.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dkp.gzhubu.top

[K02] JSON 字符串转对象
来源：http://mpd.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://wyb.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hta.jqgfzy.top

JS:   JSON.parse(s)
来源：http://hxj.hesvh.cn

TS:   JSON.parse(s)
来源：http://hhm.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aiy.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://svx.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://lgf.andypj.xyz


<!-- 参考信息 -->