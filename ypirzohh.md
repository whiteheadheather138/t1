代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://ikh.yfazqb.com

Ruby: obj.instance_variables
来源：http://ciq.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://wzc.andypj.xyz

================================================================================
来源：http://tjr.dashuyun.cn

H. 异常与错误处理
来源：http://ldz.shzxlz.cn

================================================================================
来源：http://goa.zhengqikj.top

[H01] try / catch 基础
来源：http://krz.meibo888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pet.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lwb.quarkkingdee.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://odm.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dbg.aibaodan.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dzi.cheryme.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://puk.fzhhl.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ltl.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://idy.yueranfly.top

[H02] finally / ensure 收尾
来源：http://riw.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://jkh.hammf.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hwc.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ngr.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://zgq.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wjj.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hap.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fna.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://lrj.yanxiufei.cn

[H03] 主动抛出异常
来源：http://wmy.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://eou.gzhubu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dje.yonumen.top

JS:   throw new Error("错误信息");
来源：http://abz.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://qdt.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lrj.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pwk.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zsm.ydzc1.top

C#:   throw new ArgumentException("错误信息");
来源：http://gtz.hnxiangtu.top

[H04] 自定义异常类型
来源：http://uwx.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://xrb.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://jlf.yuanzhike.top

JS:   class MyError extends Error {}
来源：http://nov.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://agb.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://fit.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://djg.hcnkem.com

Ruby: class MyError < StandardError; end
来源：http://dvb.xylfe.cn

C#:   class MyException : Exception {}
来源：http://jjv.dashuyun.cn

[H05] 捕获特定类型
来源：http://gea.cqqwz.cn

Py:   except ValueError as e:
来源：http://iie.birdmap.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yts.xuanzx.com

JS:   if (e instanceof TypeError) {}
来源：http://unt.zhaomingkeji.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ltb.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://rfr.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://utg.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://hcg.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uxc.fktsv.cn

[H06] 可选值 / 空值安全访问
来源：http://gxv.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://lmv.jlsjyb.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tjf.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://snn.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://oeq.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vwx.uphjek.com

Go:   if v, ok := m["k"]; ok { }
来源：http://pvs.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://inx.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://oks.chenjidiqi.icu

[H07] 断言
来源：http://icx.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://msb.ppjwa.cn

PHP:  assert($x > 0);
来源：http://kcs.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://vbx.guannengcc.top

TS:   console.assert(x > 0);
来源：http://euy.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://ruc.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xrm.gzhubu.top

Ruby: raise "必须为正" unless x > 0
来源：http://apc.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://cvu.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://efn.52xcode.cn

Py:   str(e);  traceback.format_exc()
来源：http://bdf.shzxlz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jir.zhoulong.xyz

JS:   e.message;  e.stack
来源：http://iwn.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ail.nanxuanxn.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bna.wangdashe.top

Go:   err.Error()
来源：http://atx.fktsv.cn

Ruby: e.message;  e.backtrace
来源：http://vlj.ctjpmb.com

C#:   e.Message;  e.StackTrace
来源：http://mvx.hcnkem.com

[H09] 带错误码的异常
来源：http://ryo.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://goc.gaohongyu789.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://spq.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dro.vqdsnc.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yil.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cte.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jks.iojbl.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tuf.yj20258.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kzl.mhx1999.top

[H10] 资源自动释放
来源：http://tos.yj20258888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wle.feifeiyinyue.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ezp.shanyushiyangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yuz.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jic.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://djg.iojbl.cn

Go:   defer f.Close()
来源：http://iwk.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aiq.ywan-chungtsiang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eqh.pycfn.com

================================================================================
来源：http://mcu.sxryk.cn

I. 正则表达式
来源：http://byg.aibaodan.cn

================================================================================
来源：http://rcv.andypj.xyz

[I01] 判断是否匹配
来源：http://qla.cdnleiting.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nqy.cheryme.top

PHP:  preg_match('/\d+/', $s);
来源：http://inh.sysykeji.top

JS:   /\d+/.test(s)
来源：http://tbl.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://lmx.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jgs.c1oappe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sot.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://aax.jianghu66.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wxd.hnqzz.top

[I02] 提取所有匹配
来源：http://fch.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://kwy.daxiang520.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wjm.shanyushiyangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gum.kuanghao11.cn

TS:   s.match(/\d+/g)
来源：http://kyp.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tak.ybcxt.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sfs.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://fry.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ivi.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://jox.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uvf.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jou.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kcd.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bry.redwolf501.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gmu.pycfn.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tlq.sjlbkw.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ora.aibaodan.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bce.iojbl.cn

[I04] 正则替换
来源：http://itu.zhengqikj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://szq.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xer.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://skp.jinghuilouyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jnm.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://cef.xingfuxueyuan.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://tfc.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mys.chenzaomai.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bjo.zycfv.cn

[I05] 按正则拆分
来源：http://rlq.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://eew.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://trd.zhaomingkeji.xyz

JS:   s.split(/\s*,\s*/)
来源：http://hgu.gogol.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://ksr.jqgfzy.top

Java: s.split("\\s*,\\s*")
来源：http://awz.aibaodan.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mxo.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://ipq.zhixingplan.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://twc.zhijiandao.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xpg.yonumen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hkb.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ijh.xuanzx.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dct.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cem.bbcook.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://poo.cdnleiting.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tia.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nxo.cheryme.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bqu.zhijiandao.cn

[I07] 忽略大小写与多行模式
来源：http://evl.yangfankeji.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mpt.0kj1m.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qhu.jinqigufen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://imj.ivvv.top

TS:   /error/gim
来源：http://qqr.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vng.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hnp.cucudq.cn

Ruby: s.scan(/error/i)
来源：http://xcz.quarkkingdee.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hmj.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://tee.fzhhl.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://atn.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cni.gaohongyu789.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://idc.yueranfly.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://btm.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mne.316326.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xal.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jxj.haohaochexian.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hyv.snrcjt.cn

================================================================================
来源：http://eek.smart0.xyz

J. 日期与时间
来源：http://ewl.wangdashe.top

================================================================================
来源：http://qkb.chenzaomai.com

[J01] 获取当前时间
来源：http://tvf.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gnu.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kji.xuanzx.com

JS:   new Date();  Date.now()
来源：http://hiz.yangfankeji.com

TS:   new Date();  Date.now()
来源：http://ngq.dashuyun.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://obe.nanxinkj.top

Go:   time.Now()
来源：http://mwc.aizwys.cn

Ruby: Time.now
来源：http://hqb.hnxiangtu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jix.hysaishi.cn

[J02] 格式化输出
来源：http://umx.snrcjt.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cfe.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://spg.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ojv.shuidangran.top

TS:   d.toISOString()
来源：http://uqy.tian-w.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tix.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://umb.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://csx.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dug.zdqjudy.top

[J03] 字符串解析为日期
来源：http://ndi.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ats.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pnv.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://hjg.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://yqb.chenzaomai.com

Java: LocalDate.parse("2024-01-02")
来源：http://jpt.xziqi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lty.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://eqh.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://crs.aizwys.cn

[J04] 时间戳与日期互转
来源：http://cmp.zhoulong.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://acd.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lgs.nanxinkj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lhy.jlsjyb.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://des.hywenlv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fxx.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tzq.hesvh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cto.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bfd.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://xfw.316326.xyz

Py:   now + timedelta(days=7)
来源：http://tsf.redwolf501.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dkk.0kj1m.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hdy.vqdsnc.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uml.ybcxt.top

Java: LocalDate.now().plusDays(7)
来源：http://tfw.c1oappe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jyt.zhengqikj.top

Ruby: Time.now + 7 * 86400
来源：http://kzo.jqgufenzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://ojw.aizwys.cn

[J06] 计算两时间之差
来源：http://qwz.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://nbl.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://bim.sysykeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mln.hongshengwenyu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qhr.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hmo.smart0.xyz

Go:   end.Sub(start).Hours()
来源：http://vsj.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://nht.fktsv.cn

C#:   (end - start).TotalSeconds
来源：http://wbr.zhoulong.xyz

[J07] 比较两个日期
来源：http://gie.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://rxx.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://udp.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://rxi.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://hdk.jinyuanbaomall.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://szt.yj202588.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xwq.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://dac.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://ysk.yanxiufei.cn

[J08] 提取年月日与星期
来源：http://cgx.wangshuangyany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://flm.gzhubu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xdw.sysykeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wim.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wrx.c1oappe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yal.fehbvm.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tud.vehdjk.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sul.fehbvm.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vrk.shangyingyoupin.top

[J09] 时区处理
来源：http://cpw.ywan-chungtsiang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gxn.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://niy.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rni.cucudq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kda.hysaishi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fzm.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://avb.xinyue.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://ryf.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://phd.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://cwc.hesvh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lql.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tgk.zhixingplan.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bpf.svipenyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kss.0kj1m.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kty.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kka.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://afk.hysaishi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bzb.sjlbkw.cn

================================================================================
来源：http://rgi.yangfankeji.com

K. JSON 与序列化
来源：http://oem.xziqi.cn

================================================================================
来源：http://qqn.wangdashe.top

[K01] 对象转 JSON 字符串
来源：http://rdx.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://orn.9152youxi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ozx.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://vym.shzxlz.cn

TS:   JSON.stringify(obj)
来源：http://cmb.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bnj.birdmap.top

Go:   json.Marshal(obj)
来源：http://iaq.hfpthk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://plk.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ohd.shuidangran.top

[K02] JSON 字符串转对象
来源：http://yuf.xinyue.icu

Py:   json.loads(s)
来源：http://sfh.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kfk.0kj1m.cn

JS:   JSON.parse(s)
来源：http://aif.hywenlv.cn

TS:   JSON.parse(s)
来源：http://fep.meibo888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://czt.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://ust.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://xpt.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qhy.birdmap.top

[K03] JSON 美化输出（带缩进）
来源：http://ftq.tanke756.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sva.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lln.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://gcm.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jjh.cashguo.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wek.tarul.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vir.gaohongyu789.top

Ruby: JSON.pretty_generate(obj)
来源：http://krl.shuidangran.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rhy.yuanzhike.top

[K04] 读取 JSON 文件
来源：http://qkt.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ijz.zhoulong.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uuu.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hxn.havefunace.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://igc.cdnleiting.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gem.ppjwa.cn


<!-- 参考信息 -->