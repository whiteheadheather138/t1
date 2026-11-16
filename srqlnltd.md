代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://tkp.jqgufenzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://enl.ppjwa.cn

[G16] 对象转数组 / 字典
来源：http://imw.ivvv.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ptn.316326.xyz

PHP:  get_object_vars($obj);
来源：http://dko.xziqi.cn

JS:   Object.entries(obj)
来源：http://imn.daria6918.cn

TS:   Object.entries(obj)
来源：http://pij.yongpay.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zps.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ewz.redwolf501.top

Ruby: obj.instance_variables
来源：http://det.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://ebh.yj20258.top

================================================================================
来源：http://xso.nanxinkj.top

H. 异常与错误处理
来源：http://jwd.xuetiantiany.cn

================================================================================
来源：http://fti.shzxlz.cn

[H01] try / catch 基础
来源：http://pkc.gaohongyu789.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pbi.c1oappe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://opd.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pji.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sxk.andypj.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xht.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zyo.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://arb.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kus.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://gtc.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://osg.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://lhf.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hnv.tanke756.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tij.nanxuanxn.top

Java: try { f(); } finally { cleanup(); }
来源：http://usm.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://cdy.kuanghao11.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zzh.wangshuangyany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oxp.cqqwz.cn

[H03] 主动抛出异常
来源：http://xcj.shanyushiyangtech.top

Py:   raise ValueError("错误信息")
来源：http://tnj.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gtg.sjlbkw.cn

JS:   throw new Error("错误信息");
来源：http://pdq.sjlbkw.cn

TS:   throw new Error("错误信息");
来源：http://fhv.nanxinkj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mdg.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qyd.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yis.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://qmb.yvedp.cn

[H04] 自定义异常类型
来源：http://myc.epnwcf.com

Py:   class MyError(Exception): pass
来源：http://ypq.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zfl.316326.xyz

JS:   class MyError extends Error {}
来源：http://tzt.yonumen.top

TS:   class MyError extends Error {}
来源：http://kbk.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://pqp.zhengqikj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://slt.jqgfzy.top

Ruby: class MyError < StandardError; end
来源：http://irx.wangdashe.top

C#:   class MyException : Exception {}
来源：http://nyc.gaohongyu789.top

[H05] 捕获特定类型
来源：http://qda.tian-w.cn

Py:   except ValueError as e:
来源：http://kpm.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kap.hammf.cn

JS:   if (e instanceof TypeError) {}
来源：http://tna.zhijiandao.cn

TS:   if (e instanceof TypeError) {}
来源：http://dhn.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://fwy.nwbrower.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nmg.tarul.cn

Ruby: rescue ArgumentError => e
来源：http://mrw.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qnx.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://mqu.cashguo.top

Py:   value = d.get("k") or default
来源：http://qbe.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://iyy.0kj1m.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ohu.kuanghao11.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yoo.gaohongyu789.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ofj.pengpengdd.cyou

Go:   if v, ok := m["k"]; ok { }
来源：http://dwi.hysaishi.cn

Ruby: d&.dig(:a, :b)
来源：http://zzx.hysaishi.cn

C#:   obj?.A?.B ?? default
来源：http://eeq.cdnleiting.top

[H07] 断言
来源：http://wfe.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://rwt.pycfn.com

PHP:  assert($x > 0);
来源：http://mum.xziqi.cn

JS:   console.assert(x > 0);
来源：http://ffa.sweek.top

TS:   console.assert(x > 0);
来源：http://zbt.0kj1m.cn

Java: assert x > 0 : "必须为正";
来源：http://ufz.sysykeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cds.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://htb.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://zme.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://kgz.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://qji.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bcx.0kj1m.cn

JS:   e.message;  e.stack
来源：http://wtz.jinghuilouyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://olz.daxiang520.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jwq.guowangkeji.top

Go:   err.Error()
来源：http://gxs.fanxiaobao.xyz

Ruby: e.message;  e.backtrace
来源：http://wzd.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://tcl.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://utr.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://olw.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://unk.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xah.dianchejie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ofp.gzhubu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wze.sufxvd.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vzi.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://vbv.epnwcf.com

C#:   // 自定义异常类中加 Code 属性
来源：http://tiy.jinyuanbaomall.cn

[H10] 资源自动释放
来源：http://lxp.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://xtx.hywenlv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wrj.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bgr.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jrb.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nbs.yj20258888.top

Go:   defer f.Close()
来源：http://emd.hesvh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fmk.yongpay.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cmk.hnxiangtu.top

================================================================================
来源：http://mev.zhaomingkeji.xyz

I. 正则表达式
来源：http://lks.bjfxy.top

================================================================================
来源：http://zjt.yvedp.cn

[I01] 判断是否匹配
来源：http://vlt.ppjwa.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eoe.gotoacloud.top

PHP:  preg_match('/\d+/', $s);
来源：http://yld.aizwys.cn

JS:   /\d+/.test(s)
来源：http://zeu.xinyue.icu

TS:   /\d+/.test(s)
来源：http://yds.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xbj.xuanzx.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hsv.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://pik.jlsjyb.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yxn.wangdashe.top

[I02] 提取所有匹配
来源：http://xao.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://kic.cqqwz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yae.ppjwa.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vkt.sjlbkw.cn

TS:   s.match(/\d+/g)
来源：http://xyl.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wyl.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://beb.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://rbp.hammf.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ker.shanyushiyangtech.top

[I03] 提取捕获分组
来源：http://bee.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wlt.hywenlv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ccq.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oxd.fengsongda.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gse.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://onf.yonumen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qwe.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rwb.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ffk.uphjek.com

[I04] 正则替换
来源：http://rlv.ppjwa.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zzo.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ewf.hywenlv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qdg.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://txe.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://tnv.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ooq.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zga.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aac.zycfv.cn

[I05] 按正则拆分
来源：http://rhg.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://rjb.hammf.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jmi.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://lop.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://dtd.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://the.sweek.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lmi.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://lpf.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lqc.jyoumei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ofp.haohaochexian.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wrl.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://axe.sysykeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hlo.ywan-chungtsiang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://psz.pengpengdd.cyou

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pqi.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://btg.pycfn.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pnh.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rmf.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://ogo.yonumen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xqx.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dyq.cheryme.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cdo.sysykeji.top

TS:   /error/gim
来源：http://nhn.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hpf.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kkp.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://sfm.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xjw.meibo888.top

[I08] 贪婪与非贪婪匹配
来源：http://zuf.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ntd.sysykeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://otx.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nuv.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fqh.zhongyouzk.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mlt.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wwe.xylfe.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lsi.yj202588.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jlt.shuidangran.top

================================================================================
来源：http://wcf.shangyingyoupin.top

J. 日期与时间
来源：http://qsy.zycfv.cn

================================================================================
来源：http://aqj.dashuyun.cn

[J01] 获取当前时间
来源：http://rfd.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dyz.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oaq.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://kwz.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://lys.nanxinkj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ppr.gogol.net.cn

Go:   time.Now()
来源：http://gre.hysaishi.cn

Ruby: Time.now
来源：http://wtg.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kcg.haohaochexian.top

[J02] 格式化输出
来源：http://imx.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://edw.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nib.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oxz.zdbjq.cn

TS:   d.toISOString()
来源：http://vcp.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ztw.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fqm.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://doh.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iiu.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://eus.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rdk.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ove.zhiwuduotai.top

JS:   new Date("2024-01-02")
来源：http://ktz.hongshengwenyu.top

TS:   new Date("2024-01-02")
来源：http://yth.vqdsnc.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ucs.shzxlz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jgp.yongpay.top

Ruby: Date.parse("2024-01-02")
来源：http://nwt.0kj1m.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ipb.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://qyy.shuidangran.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cwb.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lai.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bat.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://awr.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dpq.sxryk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yau.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lcg.gogol.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fto.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://zsd.nanxuanxn.top

Py:   now + timedelta(days=7)
来源：http://mye.xingfuxueyuan.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://bau.yongpay.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vwo.hcnkem.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vpl.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://zai.52xcode.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rdf.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://zqj.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ycc.sweek.top

[J06] 计算两时间之差
来源：http://fma.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://ccf.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://uaf.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kyo.bbcook.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qtj.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qxs.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://lwk.jinyuanbaomall.cn

Ruby: end - start                 # 返回秒数
来源：http://pie.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://try.xuetiantiany.cn

[J07] 比较两个日期
来源：http://vgs.yuanzhike.top

Py:   d1 < d2;  d1 == d2
来源：http://evr.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mle.shangyingyoupin.top

JS:   d1.getTime() < d2.getTime()
来源：http://ouq.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://nqr.hywenlv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ntv.52xcode.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ova.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wvv.jinqigufen.top

C#:   d1 < d2;  d1 == d2
来源：http://ssd.shanyushiyangkeji.top

[J08] 提取年月日与星期
来源：http://qba.ctjpmb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oki.jiagoushi.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ggs.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zvb.sysykeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lhq.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wwe.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ado.ctjpmb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fny.vqdsnc.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dct.jinqigfzy.top

[J09] 时区处理
来源：http://igy.jinghuilouyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nkw.gogol.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lsx.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://myw.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ddt.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tyo.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jko.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://qpu.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hgy.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://qpt.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oac.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xoq.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oid.ywan-chungtsiang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nbd.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gcy.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jsj.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vvu.mhx1999.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wgd.tanke756.top

================================================================================
来源：http://eon.feifeiyinyue.top

K. JSON 与序列化
来源：http://zmj.gogol.net.cn

================================================================================
来源：http://bka.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://vtf.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cpz.feifeiyinyue.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ydg.yj20258.top

JS:   JSON.stringify(obj)
来源：http://ffb.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://ffe.bbcook.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uxv.cheryme.top

Go:   json.Marshal(obj)
来源：http://jbx.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vvl.hywenlv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://myx.tianlin.xyz

[K02] JSON 字符串转对象
来源：http://bsy.xinyue.icu

Py:   json.loads(s)
来源：http://umz.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lvt.bbcook.cn

JS:   JSON.parse(s)
来源：http://pam.chenjidiqi.icu

TS:   JSON.parse(s)
来源：http://ylt.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gzx.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://dlz.jianghu66.top

Ruby: JSON.parse(s)
来源：http://hgg.uphjek.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nka.hcnkem.com

[K03] JSON 美化输出（带缩进）
来源：http://tjr.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ffr.kuanghao11.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ilc.zhijiandao.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jew.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sed.vqdsnc.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rgd.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cha.fanxiaobao.xyz


<!-- 参考信息 -->