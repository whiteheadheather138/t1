代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nna.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hbe.yj20258888.top

Java: enum Color { RED, GREEN }
来源：http://oyd.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yze.gotoacloud.top

Ruby: Color = %i[red green].freeze
来源：http://jia.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ivg.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://ren.daria6918.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://auq.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://vnp.xingfuxueyuan.xyz

JS:   Object.entries(obj)
来源：http://fzl.kuanghao11.cn

TS:   Object.entries(obj)
来源：http://kga.c1oappe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uel.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://gtu.jianghu66.top

Ruby: obj.instance_variables
来源：http://edf.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://mkx.chenlongwang.top

================================================================================
来源：http://dxn.birdmap.top

H. 异常与错误处理
来源：http://vtl.quarkkingdee.top

================================================================================
来源：http://uqc.birdmap.top

[H01] try / catch 基础
来源：http://fqz.bbcook.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sow.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://heo.havefunace.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ars.xuetiantiany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ziz.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xvp.fehbvm.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ixr.mhx1999.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://per.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://utn.xziqi.cn

[H02] finally / ensure 收尾
来源：http://kqm.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wed.quarkkingdee.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pre.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yeu.hysaishi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hvs.chenzaomai.com

Java: try { f(); } finally { cleanup(); }
来源：http://com.hysaishi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fyr.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://hpr.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qwe.jqgfzy.top

[H03] 主动抛出异常
来源：http://clh.9152youxi.cn

Py:   raise ValueError("错误信息")
来源：http://rza.dashuyun.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xiu.jyoumei.cn

JS:   throw new Error("错误信息");
来源：http://kxh.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://ppi.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kre.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ydn.xylfe.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kux.smart0.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://rnx.shuidangran.top

[H04] 自定义异常类型
来源：http://ixc.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://ukt.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://dmj.ydzc1.top

JS:   class MyError extends Error {}
来源：http://rtq.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://ajf.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://vka.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tla.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://wtm.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://kmx.yangfankeji.com

[H05] 捕获特定类型
来源：http://whz.zhoulong.xyz

Py:   except ValueError as e:
来源：http://dnb.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pcn.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://byf.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://pil.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://vqj.hnxiangtu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zwl.hesvh.cn

Ruby: rescue ArgumentError => e
来源：http://gpx.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cfv.fzhhl.top

[H06] 可选值 / 空值安全访问
来源：http://uib.yvedp.cn

Py:   value = d.get("k") or default
来源：http://ihh.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jpf.epnwcf.com

JS:   obj?.a?.b;  d ?? default
来源：http://prx.ywan-chungtsiang.top

TS:   obj?.a?.b;  d ?? default
来源：http://dtt.yangfankeji.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zvw.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://koa.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://tlw.9152youxi.cn

C#:   obj?.A?.B ?? default
来源：http://gxi.jqgufenzy.top

[H07] 断言
来源：http://qce.gaohongyu789.top

Py:   assert x > 0, "必须为正"
来源：http://ink.jyoumei.cn

PHP:  assert($x > 0);
来源：http://ubp.jinqigufen.top

JS:   console.assert(x > 0);
来源：http://rdx.birdmap.top

TS:   console.assert(x > 0);
来源：http://dbx.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://dvv.jyoumei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bca.bjfxy.top

Ruby: raise "必须为正" unless x > 0
来源：http://pyh.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://kjq.xziqi.cn

[H08] 获取错误信息与堆栈
来源：http://bmj.jianghu66.top

Py:   str(e);  traceback.format_exc()
来源：http://pph.ehwqpu.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rbs.uphjek.com

JS:   e.message;  e.stack
来源：http://mga.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lzw.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://llx.jinqigufen.top

Go:   err.Error()
来源：http://tod.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://vos.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://mws.yangfankeji.com

[H09] 带错误码的异常
来源：http://lly.pycfn.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wos.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://amn.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xbe.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wnx.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bjh.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qch.jiagoushi.top

Ruby: raise MyError.new("fail", 500)
来源：http://ovb.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uuc.fengsongda.top

[H10] 资源自动释放
来源：http://xrn.hnqzz.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nla.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yyf.hammf.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://aei.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nsp.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hnc.hfpthk.cn

Go:   defer f.Close()
来源：http://rfp.tianlin.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zjl.fanxiaobao.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gnl.52xcode.cn

================================================================================
来源：http://ncb.daria6918.cn

I. 正则表达式
来源：http://dwi.fengsongda.top

================================================================================
来源：http://xmf.jqgufenzy.top

[I01] 判断是否匹配
来源：http://yxp.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://czn.shangyingyoupin.top

PHP:  preg_match('/\d+/', $s);
来源：http://lpw.epnwcf.com

JS:   /\d+/.test(s)
来源：http://irf.sysykeji.top

TS:   /\d+/.test(s)
来源：http://ehl.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ada.iojbl.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mvz.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://hbi.cdnleiting.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ibx.xingfuxueyuan.xyz

[I02] 提取所有匹配
来源：http://ehu.gzhubu.top

Py:   re.findall(r"\d+", s)
来源：http://qiz.ydjk.org.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gku.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gfn.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://onm.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nqu.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xax.jinghuilouyu.cn

Ruby: s.scan(/\d+/)
来源：http://idu.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vui.bjfxy.top

[I03] 提取捕获分组
来源：http://bfi.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sou.jinyuanbaomall.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vbn.316326.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mvc.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bie.sweek.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://woi.nwbrower.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://btx.quarkkingdee.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wmh.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://erj.shuidangran.top

[I04] 正则替换
来源：http://ebw.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nqd.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ema.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vmb.zhongyouzk.top

TS:   s.replace(/\d+/g, "#")
来源：http://mpe.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://raa.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://hiq.zhongyouzk.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hus.bjfxy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rja.zhijiandao.cn

[I05] 按正则拆分
来源：http://iek.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ikr.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gkq.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://nvv.xuetiantiany.cn

TS:   s.split(/\s*,\s*/)
来源：http://myf.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://fxq.ctjpmb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tmt.ybcxt.top

Ruby: s.split(/\s*,\s*/)
来源：http://shz.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qmq.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nsx.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oad.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gns.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://auv.cheryme.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tzi.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tql.xuanzx.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xcc.quarkkingdee.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cof.hesvh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wie.zhijiandao.cn

[I07] 忽略大小写与多行模式
来源：http://bqi.gzhubu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://opz.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yov.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mpm.zhixingplan.top

TS:   /error/gim
来源：http://vdp.zhongyouzk.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ebw.ctjpmb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vxl.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://udy.cucudq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yfb.ybcxt.top

[I08] 贪婪与非贪婪匹配
来源：http://qkz.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ohq.aizwys.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://usb.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tjq.cucudq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iev.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://stz.0kj1m.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uto.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ius.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ctc.shangyingyoupin.top

================================================================================
来源：http://cmt.hfpthk.cn

J. 日期与时间
来源：http://wcz.mhx1999.top

================================================================================
来源：http://lco.hywenlv.cn

[J01] 获取当前时间
来源：http://sft.shanyushiyangtech.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fmw.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ayv.zhixingplan.top

JS:   new Date();  Date.now()
来源：http://hfs.jiagoushi.top

TS:   new Date();  Date.now()
来源：http://zsj.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fop.feifeiyinyue.top

Go:   time.Now()
来源：http://mgc.meibo888.top

Ruby: Time.now
来源：http://mnm.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jgq.ehwqpu.com

[J02] 格式化输出
来源：http://xex.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rbt.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fvl.gotoacloud.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cur.jqgufenzy.top

TS:   d.toISOString()
来源：http://ash.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://asm.zhoulong.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://urn.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nys.316326.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rrq.iojbl.cn

[J03] 字符串解析为日期
来源：http://qth.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kpg.haohaochexian.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kvx.bjfxy.top

JS:   new Date("2024-01-02")
来源：http://clk.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://uiw.yangfankeji.com

Java: LocalDate.parse("2024-01-02")
来源：http://jcx.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hwn.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://lba.hongshengwenyu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kde.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://zpm.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uwf.ydzc1.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vqs.sjlbkw.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pbc.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rsi.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ouk.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ytl.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xeg.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ujt.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://qus.daxiang520.top

Py:   now + timedelta(days=7)
来源：http://yda.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://adt.tianlin.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oep.xylfe.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ebj.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://gsz.shuidangran.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ikb.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://lch.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://zyc.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://nhw.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://cbg.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://oxw.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iyg.daria6918.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gsh.bjfxy.top

Java: Duration.between(start, end).toSeconds()
来源：http://ufo.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://tza.shangyingyoupin.top

Ruby: end - start                 # 返回秒数
来源：http://qhj.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://igv.hongshengwenyu.top

[J07] 比较两个日期
来源：http://vfz.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://brr.ydjk.org.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yny.xuetiantiany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dub.zhongyouzk.top

TS:   d1.getTime() < d2.getTime()
来源：http://bod.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zgr.sjlbkw.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nqv.hammf.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ftb.yanxiufei.cn

C#:   d1 < d2;  d1 == d2
来源：http://qqk.tarul.cn

[J08] 提取年月日与星期
来源：http://zlm.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pwa.yvedp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://adk.vehdjk.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jiy.nanxinkj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hdj.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://non.nwbrower.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lyb.ybcxt.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ret.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xdc.shzxlz.cn

[J09] 时区处理
来源：http://xvd.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://llt.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vbi.vqdsnc.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nbr.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://okg.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ote.tanke756.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uci.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wll.shanyushiyangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lfe.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://khg.fanxiaobao.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://edf.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uix.hnqzz.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jsn.gzhubu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vbo.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://afm.guowangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ntg.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ejm.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://auo.jinqigufen.top

================================================================================
来源：http://axc.cheryme.top

K. JSON 与序列化
来源：http://yag.tarul.cn

================================================================================
来源：http://ldu.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://qns.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pfj.kuanghao11.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jdi.jlsjyb.cn

JS:   JSON.stringify(obj)
来源：http://nkb.yuanzhike.top

TS:   JSON.stringify(obj)
来源：http://wiy.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wqa.hcnkem.com

Go:   json.Marshal(obj)
来源：http://aso.nanxinkj.top

Ruby: obj.to_json                                     // require "json"
来源：http://tmt.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://vvb.sysykeji.top

[K02] JSON 字符串转对象
来源：http://gbx.ivvv.top

Py:   json.loads(s)
来源：http://feb.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://msj.hnxiangtu.top

JS:   JSON.parse(s)
来源：http://wlw.fehbvm.com

TS:   JSON.parse(s)
来源：http://gqm.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xvh.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://pje.gzhubu.top

Ruby: JSON.parse(s)
来源：http://jgp.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ccw.dashuyun.cn

[K03] JSON 美化输出（带缩进）
来源：http://agz.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vhn.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://opr.svipenyu.cn


<!-- 参考信息 -->