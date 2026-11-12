代发 wailian999

C#:   record User(string Name, int Age);
来源：http://pxb.yvedp.cn

[G15] 枚举
来源：http://hwp.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://prd.snrcjt.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rpm.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tbi.haohaochexian.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pxu.shuidangran.top

Java: enum Color { RED, GREEN }
来源：http://fch.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mce.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://snm.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kbe.vqdsnc.cn

[G16] 对象转数组 / 字典
来源：http://dtq.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dlg.wangdashe.top

PHP:  get_object_vars($obj);
来源：http://eha.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://qax.shzxlz.cn

TS:   Object.entries(obj)
来源：http://new.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tde.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://olr.aibaodan.cn

Ruby: obj.instance_variables
来源：http://bzt.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://alz.jqgfzy.top

================================================================================
来源：http://zvd.yfazqb.com

H. 异常与错误处理
来源：http://nzf.zhaomingkeji.xyz

================================================================================
来源：http://xrj.dianchejie.cn

[H01] try / catch 基础
来源：http://rlp.sweek.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kkz.hongshengwenyu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://szr.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oso.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ldm.smart0.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wmw.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gho.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vgi.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yqa.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://njy.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://zyh.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://xza.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://roz.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ydb.xylfe.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xxq.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://fyw.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vtc.zhongyouzk.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://upd.guowangkeji.top

[H03] 主动抛出异常
来源：http://zkf.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://odn.fehbvm.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://faj.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://asv.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://jpd.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://pkk.shuidangran.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kiq.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://loo.c1oappe.top

C#:   throw new ArgumentException("错误信息");
来源：http://ahv.xylfe.cn

[H04] 自定义异常类型
来源：http://sul.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://lam.fengsongda.top

PHP:  class MyError extends RuntimeException {}
来源：http://duu.ctjpmb.com

JS:   class MyError extends Error {}
来源：http://gvs.xinyue.icu

TS:   class MyError extends Error {}
来源：http://jdc.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://nmz.yvedp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aue.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://zie.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://uup.snrcjt.cn

[H05] 捕获特定类型
来源：http://kjy.jlsjyb.cn

Py:   except ValueError as e:
来源：http://bzb.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bty.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://nds.ybcxt.top

TS:   if (e instanceof TypeError) {}
来源：http://hip.hysaishi.cn

Java: catch (IOException | SQLException e) {}
来源：http://oda.cqqwz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pcr.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://kxq.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xsl.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://zul.daria6918.cn

Py:   value = d.get("k") or default
来源：http://sqi.nanxinkj.top

PHP:  $v = $d["k"] ?? null;
来源：http://hbu.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://xwr.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ajy.hfpthk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rfw.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dqw.fehbvm.com

Ruby: d&.dig(:a, :b)
来源：http://lqf.zhixingplan.top

C#:   obj?.A?.B ?? default
来源：http://azp.zycfv.cn

[H07] 断言
来源：http://vah.daria6918.cn

Py:   assert x > 0, "必须为正"
来源：http://ogo.9152youxi.cn

PHP:  assert($x > 0);
来源：http://nsd.fktsv.cn

JS:   console.assert(x > 0);
来源：http://giy.quarkkingdee.top

TS:   console.assert(x > 0);
来源：http://hpl.yj202588.top

Java: assert x > 0 : "必须为正";
来源：http://crj.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bde.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://cae.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://prb.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://kwb.bbcook.cn

Py:   str(e);  traceback.format_exc()
来源：http://fut.yfazqb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ktz.aizwys.cn

JS:   e.message;  e.stack
来源：http://qsu.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gbq.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oau.xuanzx.com

Go:   err.Error()
来源：http://pgt.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://fjz.yueranfly.top

C#:   e.Message;  e.StackTrace
来源：http://esj.shanyushiyangkeji.top

[H09] 带错误码的异常
来源：http://eaa.vehdjk.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qbh.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://jsv.birdmap.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fqf.cashguo.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://npz.ybcxt.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lgn.kuanghao11.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lze.zhoulong.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://xyf.kuanghao11.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jcn.zhijiandao.cn

[H10] 资源自动释放
来源：http://hxj.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jyt.nanxuanxn.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://prw.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://liq.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wtm.shanyushiyangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://thh.guowangkeji.top

Go:   defer f.Close()
来源：http://ojn.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wpi.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cwn.jqgfzy.top

================================================================================
来源：http://hdj.daria6918.cn

I. 正则表达式
来源：http://cij.cucudq.cn

================================================================================
来源：http://iqi.ctjpmb.com

[I01] 判断是否匹配
来源：http://hse.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wif.yfazqb.com

PHP:  preg_match('/\d+/', $s);
来源：http://qgz.sjlbkw.cn

JS:   /\d+/.test(s)
来源：http://mli.bbcook.cn

TS:   /\d+/.test(s)
来源：http://edx.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oqw.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ant.aizwys.cn

Ruby: s.match?(/\d+/)
来源：http://sdq.svipenyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://isz.jlsjyb.cn

[I02] 提取所有匹配
来源：http://sue.sweek.top

Py:   re.findall(r"\d+", s)
来源：http://rqr.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pbi.yj202588.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nhv.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://zsf.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eix.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mcn.daria6918.cn

Ruby: s.scan(/\d+/)
来源：http://gvx.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://omv.hesvh.cn

[I03] 提取捕获分组
来源：http://vjk.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vvx.jiagoushi.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jqs.zhijiandao.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jjl.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vlm.feifeiyinyue.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yje.jiagoushi.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pjj.wangshuangyany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eog.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cah.jqgufenzy.top

[I04] 正则替换
来源：http://wfn.ydjk.org.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gby.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eqb.sweek.top

JS:   s.replace(/\d+/g, "#")
来源：http://tfc.fktsv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kjw.jqgfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://dbw.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ghh.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dhw.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://myk.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://sui.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://nii.zhaomingkeji.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lcu.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://tkk.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://igg.sysykeji.top

Java: s.split("\\s*,\\s*")
来源：http://sxk.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uop.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://gif.hywenlv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://evd.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jar.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ssw.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dfh.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uxt.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yoc.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nhy.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cpr.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rnc.fzhhl.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lzk.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://vxe.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yrw.redwolf501.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wbg.jqgufenzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cub.zhaomingkeji.xyz

TS:   /error/gim
来源：http://gja.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://txg.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kwb.jlsjyb.cn

Ruby: s.scan(/error/i)
来源：http://klv.ybcxt.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://edb.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://non.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fhm.mhx1999.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tdo.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://spp.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://khl.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jkl.fehbvm.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://whe.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vbk.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mfj.jqgufenzy.top

================================================================================
来源：http://ors.9152youxi.cn

J. 日期与时间
来源：http://ovw.hfpthk.cn

================================================================================
来源：http://hny.tian-w.cn

[J01] 获取当前时间
来源：http://pra.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ngf.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ugf.yj202588.top

JS:   new Date();  Date.now()
来源：http://knq.yueranfly.top

TS:   new Date();  Date.now()
来源：http://cuu.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://fdi.hywenlv.cn

Go:   time.Now()
来源：http://cpe.gzhubu.top

Ruby: Time.now
来源：http://kyw.zhiwuduotai.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pso.tian-w.cn

[J02] 格式化输出
来源：http://csj.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kfr.316326.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iiz.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lmt.wangshuangyany.cn

TS:   d.toISOString()
来源：http://sxs.cqqwz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://maz.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zsa.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rnk.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fgb.havefunace.top

[J03] 字符串解析为日期
来源：http://ddf.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qwk.gogol.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bfc.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://xse.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://lxo.pycfn.com

Java: LocalDate.parse("2024-01-02")
来源：http://syt.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tfg.nwbrower.top

Ruby: Date.parse("2024-01-02")
来源：http://ebp.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dzf.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://ceh.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tph.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xzv.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nfi.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nti.yuxming.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fxz.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hvm.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kil.52xcode.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://voc.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://krz.ydzc1.top

Py:   now + timedelta(days=7)
来源：http://odi.wangdashe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tdl.tanke756.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://udy.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pkf.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://knz.zhoulong.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hkm.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://pkw.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yrj.yangfankeji.com

[J06] 计算两时间之差
来源：http://hqk.zycfv.cn

Py:   (end - start).total_seconds()
来源：http://ekw.fehbvm.com

PHP:  $end->diff($start)->days;
来源：http://cik.vehdjk.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bez.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fij.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://coh.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://kpr.tianlin.xyz

Ruby: end - start                 # 返回秒数
来源：http://eoo.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://liu.ydzc1.top

[J07] 比较两个日期
来源：http://tar.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ncq.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://evo.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zgm.vehdjk.com

TS:   d1.getTime() < d2.getTime()
来源：http://daa.hywenlv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zsg.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tlv.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mxl.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://qtu.dianchejie.cn

[J08] 提取年月日与星期
来源：http://bph.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vfp.shzxlz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ygg.zhijiandao.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gsm.zhiwuduotai.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xmn.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ifg.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hob.xziqi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gaz.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ogo.shanyushiyangtech.top

[J09] 时区处理
来源：http://zra.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pny.aibaodan.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://avc.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vcn.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vog.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://asb.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fbx.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mlo.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hif.sufxvd.cn

[J10] 取今天 / 本月第一天
来源：http://xwe.yvedp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lyz.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uoj.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eqq.fehbvm.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://htw.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dxw.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eoj.yj20258888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vri.svipenyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lfz.shanyushiyangkeji.top

================================================================================
来源：http://jbp.nanxinkj.top

K. JSON 与序列化
来源：http://wda.haohaochexian.top

================================================================================
来源：http://sbm.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://sbp.svipenyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://otu.meibo888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iea.zhiwuduotai.top

JS:   JSON.stringify(obj)
来源：http://ctd.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://xue.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ucx.shanyushiyangkeji.top

Go:   json.Marshal(obj)
来源：http://rlq.jinqigfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://bbn.fzhhl.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nkz.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://nnu.yongpay.top

Py:   json.loads(s)
来源：http://ist.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://edt.zhongyouzk.top

JS:   JSON.parse(s)
来源：http://yvy.gzhubu.top

TS:   JSON.parse(s)
来源：http://nbo.redwolf501.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cgt.hywenlv.cn

Go:   json.Unmarshal(data, &v)
来源：http://llt.yueranfly.top

Ruby: JSON.parse(s)
来源：http://fct.andypj.xyz


<!-- 参考信息 -->