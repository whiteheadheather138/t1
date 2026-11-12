代发 wailian999

PHP:  get_object_vars($obj);
来源：http://qpg.pycfn.com

JS:   Object.entries(obj)
来源：http://udx.shuidangran.top

TS:   Object.entries(obj)
来源：http://mxb.yj20258.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qph.jinyuanbaomall.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rbh.xziqi.cn

Ruby: obj.instance_variables
来源：http://zfh.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://dff.wangdashe.top

================================================================================
来源：http://loi.zhongyouzk.top

H. 异常与错误处理
来源：http://xpf.hnqzz.top

================================================================================
来源：http://tyd.hnqzz.top

[H01] try / catch 基础
来源：http://srr.yvedp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wlw.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wqf.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xvd.nanxuanxn.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rph.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://den.316326.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mxl.fzhhl.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xin.tanke756.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kzj.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://wgg.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tzw.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ieu.meibo888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bbe.cdnleiting.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tbp.zhixingplan.top

Java: try { f(); } finally { cleanup(); }
来源：http://mwm.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ple.daria6918.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dds.hammf.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://aah.hywenlv.cn

[H03] 主动抛出异常
来源：http://tkg.chenlongwang.top

Py:   raise ValueError("错误信息")
来源：http://vqi.hesvh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kjt.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://vmg.zdbjq.cn

TS:   throw new Error("错误信息");
来源：http://dux.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bhi.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://goy.cashguo.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ifw.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://jtq.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://bvr.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://ffo.yongpay.top

PHP:  class MyError extends RuntimeException {}
来源：http://uyi.shuidangran.top

JS:   class MyError extends Error {}
来源：http://loc.yongpay.top

TS:   class MyError extends Error {}
来源：http://phu.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://toj.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zai.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://iwc.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://hiw.aibaodan.cn

[H05] 捕获特定类型
来源：http://eqq.gotoacloud.top

Py:   except ValueError as e:
来源：http://hqa.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gun.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://one.chenzaomai.com

TS:   if (e instanceof TypeError) {}
来源：http://xxc.hfpthk.cn

Java: catch (IOException | SQLException e) {}
来源：http://mwu.sufxvd.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kdx.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://owk.yueranfly.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ibb.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://pnz.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://qfu.hywenlv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hot.zhixingplan.top

JS:   obj?.a?.b;  d ?? default
来源：http://foz.hongshengwenyu.top

TS:   obj?.a?.b;  d ?? default
来源：http://xsr.sysykeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iwm.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://twt.nwbrower.top

Ruby: d&.dig(:a, :b)
来源：http://epb.cqqwz.cn

C#:   obj?.A?.B ?? default
来源：http://ori.vehdjk.com

[H07] 断言
来源：http://xrl.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://gte.ydjk.org.cn

PHP:  assert($x > 0);
来源：http://ync.guowangkeji.top

JS:   console.assert(x > 0);
来源：http://yky.hongshengwenyu.top

TS:   console.assert(x > 0);
来源：http://zzq.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://gzn.xingfuxueyuan.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://brv.fehbvm.com

Ruby: raise "必须为正" unless x > 0
来源：http://yvu.sysykeji.top

C#:   Debug.Assert(x > 0);
来源：http://wiu.9152youxi.cn

[H08] 获取错误信息与堆栈
来源：http://ton.svipenyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://qxc.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eua.redwolf501.top

JS:   e.message;  e.stack
来源：http://fhc.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gmt.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vhr.havefunace.top

Go:   err.Error()
来源：http://zmr.cheryme.top

Ruby: e.message;  e.backtrace
来源：http://rlz.daria6918.cn

C#:   e.Message;  e.StackTrace
来源：http://nvu.gaohongyu789.top

[H09] 带错误码的异常
来源：http://itd.ybcxt.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://epk.yuxming.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bpu.chenzaomai.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oyx.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gxu.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dcv.ybcxt.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dus.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://urh.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bvm.shuidangran.top

[H10] 资源自动释放
来源：http://trp.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://esg.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zal.ywan-chungtsiang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mqt.xuetiantiany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qsh.hesvh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jxh.epnwcf.com

Go:   defer f.Close()
来源：http://rjs.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nyk.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uzf.pengpengdd.cyou

================================================================================
来源：http://rmh.jqgufenzy.top

I. 正则表达式
来源：http://trk.0kj1m.cn

================================================================================
来源：http://ort.sufxvd.cn

[I01] 判断是否匹配
来源：http://odq.redwolf501.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://unz.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zdz.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://tme.xuetiantiany.cn

TS:   /\d+/.test(s)
来源：http://jkw.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ynd.yj20258888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zxl.jinqigufen.top

Ruby: s.match?(/\d+/)
来源：http://vlz.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dnu.dashuyun.cn

[I02] 提取所有匹配
来源：http://umb.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://xev.jyoumei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tpm.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://osv.hongshengwenyu.top

TS:   s.match(/\d+/g)
来源：http://kzi.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cfw.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fqk.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://jcr.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vlq.dashuyun.cn

[I03] 提取捕获分组
来源：http://yrr.chenlongwang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zrj.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oll.cucudq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dvo.jqgfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bml.jiagoushi.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pcs.fengsongda.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xdt.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yia.yj20258.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ixi.tian-w.cn

[I04] 正则替换
来源：http://dat.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rfj.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dbc.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xre.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xnk.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://wvk.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ctw.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vsm.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sjy.hnqzz.top

[I05] 按正则拆分
来源：http://pyv.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jif.yvedp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gmb.tianlin.xyz

JS:   s.split(/\s*,\s*/)
来源：http://nfe.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://dgf.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://dln.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://juw.cashguo.top

Ruby: s.split(/\s*,\s*/)
来源：http://avo.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xrz.fehbvm.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pan.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hse.dashuyun.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mvk.cheryme.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gdf.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cju.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yts.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tpm.feifeiyinyue.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iox.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xur.jinyuanbaomall.cn

[I07] 忽略大小写与多行模式
来源：http://hkz.hysaishi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uqw.fktsv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://olg.zdqjudy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bjm.jlsjyb.cn

TS:   /error/gim
来源：http://art.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iav.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dre.shuidangran.top

Ruby: s.scan(/error/i)
来源：http://dgq.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rao.jyoumei.cn

[I08] 贪婪与非贪婪匹配
来源：http://lky.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ssq.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cxg.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nhh.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vsw.havefunace.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rvm.pycfn.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gfg.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ziw.yangfankeji.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rqj.zhijiandao.cn

================================================================================
来源：http://ehh.havefunace.top

J. 日期与时间
来源：http://vtn.yuanzhike.top

================================================================================
来源：http://sox.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://ray.fengsongda.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wzg.52xcode.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rsa.yfazqb.com

JS:   new Date();  Date.now()
来源：http://pvj.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://wbr.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://hrx.aizwys.cn

Go:   time.Now()
来源：http://fsl.cheryme.top

Ruby: Time.now
来源：http://uzi.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ktx.yongpay.top

[J02] 格式化输出
来源：http://nwa.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://msi.chenjidiqi.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mvf.yueranfly.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bfb.zycfv.cn

TS:   d.toISOString()
来源：http://mxn.jiagoushi.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ges.chenlongwang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yau.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lqv.wangshuangyany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nqq.yfazqb.com

[J03] 字符串解析为日期
来源：http://yfa.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jnd.zhaomingkeji.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xih.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://ous.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://sbq.hywenlv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fnv.vqdsnc.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zcz.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://gnw.snrcjt.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xmz.xziqi.cn

[J04] 时间戳与日期互转
来源：http://ntu.zdbjq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rbw.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uwh.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://whd.fzhhl.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ked.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vmv.gzhubu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wcy.nanxinkj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nfr.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://itz.yfazqb.com

[J05] 时间加减（加 7 天）
来源：http://ebi.meibo888.top

Py:   now + timedelta(days=7)
来源：http://jcd.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://jud.chenlongwang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dtt.hnqzz.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pfw.jinqigufen.top

Java: LocalDate.now().plusDays(7)
来源：http://bux.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iss.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://uhp.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lcz.yuanzhike.top

[J06] 计算两时间之差
来源：http://gvp.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://uzp.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://hvs.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kou.ctjpmb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gll.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://bik.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://njp.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://swb.fehbvm.com

C#:   (end - start).TotalSeconds
来源：http://xqz.fktsv.cn

[J07] 比较两个日期
来源：http://afy.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://vgl.gotoacloud.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rlt.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ens.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bxp.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xne.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://utm.hywenlv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ura.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://gqi.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://oth.gotoacloud.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wah.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ymq.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pat.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://idx.ydzc1.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rhv.pengpengdd.cyou

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ihr.bjfxy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uep.shzxlz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ojf.yanxiufei.cn

[J09] 时区处理
来源：http://ljl.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://unk.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xvs.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ysw.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iqg.hammf.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://evr.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cgr.andypj.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://yjr.feifeiyinyue.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mkk.sysykeji.top

[J10] 取今天 / 本月第一天
来源：http://kdb.jyoumei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dlf.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lhg.c1oappe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://amx.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pgk.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xgr.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://myk.dashuyun.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fhm.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vyg.havefunace.top

================================================================================
来源：http://tmq.sxryk.cn

K. JSON 与序列化
来源：http://vuz.52xcode.cn

================================================================================
来源：http://emg.jinghuilouyu.cn

[K01] 对象转 JSON 字符串
来源：http://vjv.hnqzz.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qer.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dqp.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://hxg.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://luh.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eqz.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://kmv.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dcr.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cji.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://dcj.sweek.top

Py:   json.loads(s)
来源：http://fmj.yongpay.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://onx.xuanzx.com

JS:   JSON.parse(s)
来源：http://mhr.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://tdi.ctjpmb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://phe.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://hce.ehwqpu.com

Ruby: JSON.parse(s)
来源：http://dnf.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bvq.jyoumei.cn

[K03] JSON 美化输出（带缩进）
来源：http://wif.fanxiaobao.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bgf.yfazqb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hbd.fanxiaobao.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://pde.yuxming.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ahd.cucudq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mhu.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hud.birdmap.top

Ruby: JSON.pretty_generate(obj)
来源：http://ati.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yil.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://gob.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://urd.bjfxy.top


<!-- 参考信息 -->