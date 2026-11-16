代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qqx.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xxp.cheryme.top

Java: enum Color { RED, GREEN }
来源：http://aog.snrcjt.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xvk.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://tce.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tup.ydzc1.top

[G16] 对象转数组 / 字典
来源：http://quz.feifeiyinyue.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wdz.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://szx.fzhhl.top

JS:   Object.entries(obj)
来源：http://vcj.jiagoushi.top

TS:   Object.entries(obj)
来源：http://lep.c1oappe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://axm.sweek.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://izv.gotoacloud.top

Ruby: obj.instance_variables
来源：http://pxt.chenlongwang.top

C#:   // 用反射或 System.Text.Json
来源：http://dfg.yj202588.top

================================================================================
来源：http://bnq.dashuyun.cn

H. 异常与错误处理
来源：http://ber.fanxiaobao.xyz

================================================================================
来源：http://fyt.zdqjudy.top

[H01] try / catch 基础
来源：http://wnz.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rhs.sjlbkw.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kxd.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vxx.chenlongwang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://obw.zhongyouzk.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ytx.yonumen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uyo.shzxlz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eda.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tqo.zhijiandao.cn

[H02] finally / ensure 收尾
来源：http://dhv.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dxm.cashguo.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://luw.guowangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://grl.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ywd.9152youxi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qid.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://roy.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kdw.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vig.uphjek.com

[H03] 主动抛出异常
来源：http://eza.pycfn.com

Py:   raise ValueError("错误信息")
来源：http://wqp.xuanzx.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jdu.hammf.cn

JS:   throw new Error("错误信息");
来源：http://yxt.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://equ.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://cwy.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fic.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yoo.zdqjudy.top

C#:   throw new ArgumentException("错误信息");
来源：http://qlf.zhengqikj.top

[H04] 自定义异常类型
来源：http://rff.xinyue.icu

Py:   class MyError(Exception): pass
来源：http://als.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://tol.shuidangran.top

JS:   class MyError extends Error {}
来源：http://tnx.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://evv.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://drd.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fae.iojbl.cn

Ruby: class MyError < StandardError; end
来源：http://xnj.hnqzz.top

C#:   class MyException : Exception {}
来源：http://apk.jinqigufen.top

[H05] 捕获特定类型
来源：http://hmh.dashuyun.cn

Py:   except ValueError as e:
来源：http://iqz.52xcode.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://frr.zhijiandao.cn

JS:   if (e instanceof TypeError) {}
来源：http://bxo.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://zct.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://dmg.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wzt.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://bta.guowangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vwg.sjlbkw.cn

[H06] 可选值 / 空值安全访问
来源：http://shu.ivvv.top

Py:   value = d.get("k") or default
来源：http://qjf.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://vpy.shanyushiyangtech.top

JS:   obj?.a?.b;  d ?? default
来源：http://doh.zdbjq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wzm.aizwys.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ntj.shzxlz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kuk.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://eqm.zdbjq.cn

C#:   obj?.A?.B ?? default
来源：http://lod.pengpengdd.cyou

[H07] 断言
来源：http://vhl.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://uqf.jyoumei.cn

PHP:  assert($x > 0);
来源：http://eym.yvedp.cn

JS:   console.assert(x > 0);
来源：http://egn.pycfn.com

TS:   console.assert(x > 0);
来源：http://lsh.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://yba.ybcxt.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pvx.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://utk.zhixingplan.top

C#:   Debug.Assert(x > 0);
来源：http://czi.guowangkeji.top

[H08] 获取错误信息与堆栈
来源：http://uua.shanyushiyangtech.top

Py:   str(e);  traceback.format_exc()
来源：http://fta.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gsa.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://rfj.yfazqb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ita.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ylf.sjlbkw.cn

Go:   err.Error()
来源：http://giu.ydjk.org.cn

Ruby: e.message;  e.backtrace
来源：http://lzn.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://ijg.dashuyun.cn

[H09] 带错误码的异常
来源：http://thb.xingfuxueyuan.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qsj.xylfe.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wpe.yongpay.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bmx.uphjek.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xzm.andypj.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yiy.quarkkingdee.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ukj.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://swc.ywan-chungtsiang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fgf.sxryk.cn

[H10] 资源自动释放
来源：http://rpk.jinqigfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ghj.cqqwz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lid.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mvl.yanxiufei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gcy.cheryme.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ken.xziqi.cn

Go:   defer f.Close()
来源：http://qdj.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ywa.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uqu.bbcook.cn

================================================================================
来源：http://lhg.fengsongda.top

I. 正则表达式
来源：http://xfx.ehwqpu.com

================================================================================
来源：http://exy.fzhhl.top

[I01] 判断是否匹配
来源：http://ind.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qhr.zhengqikj.top

PHP:  preg_match('/\d+/', $s);
来源：http://vny.snrcjt.cn

JS:   /\d+/.test(s)
来源：http://nzn.nwbrower.top

TS:   /\d+/.test(s)
来源：http://uir.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lui.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tqr.gzhubu.top

Ruby: s.match?(/\d+/)
来源：http://yep.birdmap.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wym.havefunace.top

[I02] 提取所有匹配
来源：http://fge.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://qlk.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jje.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ihv.yj202588.top

TS:   s.match(/\d+/g)
来源：http://tsd.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uiz.shuidangran.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ffj.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://noh.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yre.jianghu66.top

[I03] 提取捕获分组
来源：http://ulz.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rdm.c1oappe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dte.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lrn.nanxinkj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oog.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bde.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bdo.tanke756.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ihb.316326.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ftf.xziqi.cn

[I04] 正则替换
来源：http://mjw.mhx1999.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lkv.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jeq.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://uvh.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://tjd.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://ghv.xuanzx.com

Go:   re.ReplaceAllString(s, "#")
来源：http://mpu.vqdsnc.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://biq.havefunace.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hvt.uphjek.com

[I05] 按正则拆分
来源：http://rtc.hesvh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bpm.zhengqikj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://upf.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://mev.daria6918.cn

TS:   s.split(/\s*,\s*/)
来源：http://nwi.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://rjr.smart0.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xpj.shangyingyoupin.top

Ruby: s.split(/\s*,\s*/)
来源：http://xgw.shanyushiyangtech.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://scu.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://are.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wdh.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xem.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jvz.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ueh.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bde.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://meq.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://brk.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ezg.jqgufenzy.top

[I07] 忽略大小写与多行模式
来源：http://gvt.hfpthk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yvq.316326.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://srg.zycfv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qhp.yj202588.top

TS:   /error/gim
来源：http://rmb.hesvh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xdb.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rxv.cashguo.top

Ruby: s.scan(/error/i)
来源：http://qby.zhijiandao.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iau.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://cwy.ehwqpu.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bwi.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vgb.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mkm.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cpk.nwbrower.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://auy.fzhhl.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jaf.ppjwa.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jmi.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nbu.hcnkem.com

================================================================================
来源：http://wyi.shanyushiyangtech.top

J. 日期与时间
来源：http://lnq.haohaochexian.top

================================================================================
来源：http://bhv.yj202588.top

[J01] 获取当前时间
来源：http://tqi.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ogf.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aod.chenzaomai.com

JS:   new Date();  Date.now()
来源：http://wmg.hnxiangtu.top

TS:   new Date();  Date.now()
来源：http://efw.pengpengdd.cyou

Java: LocalDateTime.now();  Instant.now()
来源：http://lqp.yongpay.top

Go:   time.Now()
来源：http://apf.zycfv.cn

Ruby: Time.now
来源：http://gic.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bfi.jqgfzy.top

[J02] 格式化输出
来源：http://lpu.yj20258888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aef.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nbo.hysaishi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xgg.havefunace.top

TS:   d.toISOString()
来源：http://dnh.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://akf.yj20258888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ulq.xylfe.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pae.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wfp.wangdashe.top

[J03] 字符串解析为日期
来源：http://aap.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://boc.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qhr.tian-w.cn

JS:   new Date("2024-01-02")
来源：http://odj.feifeiyinyue.top

TS:   new Date("2024-01-02")
来源：http://eik.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pqf.sysykeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xlh.nanxuanxn.top

Ruby: Date.parse("2024-01-02")
来源：http://dua.cdnleiting.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wfi.yj20258888.top

[J04] 时间戳与日期互转
来源：http://ety.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cmw.yvedp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ysg.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://thd.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rlj.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mga.zdqjudy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://asv.sjlbkw.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kqe.jianghu66.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uvs.iojbl.cn

[J05] 时间加减（加 7 天）
来源：http://aih.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://hqs.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jls.kuanghao11.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zvg.jqgfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rml.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://jiv.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yme.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://uuh.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://spo.sweek.top

[J06] 计算两时间之差
来源：http://dmm.jinyuanbaomall.cn

Py:   (end - start).total_seconds()
来源：http://dly.shanyushiyangkeji.top

PHP:  $end->diff($start)->days;
来源：http://jin.feifeiyinyue.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hcs.epnwcf.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pzg.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://pkj.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://sxh.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://ovi.shuidangran.top

C#:   (end - start).TotalSeconds
来源：http://xjp.gotoacloud.top

[J07] 比较两个日期
来源：http://yuo.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://ahd.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fxv.9152youxi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cry.xuetiantiany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wpq.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fwc.zhijiandao.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tbs.xylfe.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hpk.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://qdc.zdbjq.cn

[J08] 提取年月日与星期
来源：http://qhv.cqqwz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zfx.jiagoushi.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bef.ybcxt.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xlg.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bld.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mez.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qzn.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kra.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zre.pycfn.com

[J09] 时区处理
来源：http://qxc.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wmc.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uth.xuanzx.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xjf.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mvg.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yyj.snrcjt.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tpu.hcnkem.com

Ruby: Time.now.getlocal("+08:00")
来源：http://hii.chenjidiqi.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pzs.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://ecg.smart0.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://jbd.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qwn.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://joj.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://opl.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xlo.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ead.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dno.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xjq.shanyushiyangtech.top

================================================================================
来源：http://pxf.cucudq.cn

K. JSON 与序列化
来源：http://orh.hesvh.cn

================================================================================
来源：http://jzf.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://aip.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qgj.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xru.yonumen.top

JS:   JSON.stringify(obj)
来源：http://alp.jyoumei.cn

TS:   JSON.stringify(obj)
来源：http://bhh.ehwqpu.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ygz.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://oep.shzxlz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bwv.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://feo.daria6918.cn

[K02] JSON 字符串转对象
来源：http://pda.shuidangran.top

Py:   json.loads(s)
来源：http://aat.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gcv.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://xfu.yj20258888.top

TS:   JSON.parse(s)
来源：http://zll.nanxuanxn.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jbg.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://hzi.sjlbkw.cn

Ruby: JSON.parse(s)
来源：http://kep.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://npr.yangfankeji.com

[K03] JSON 美化输出（带缩进）
来源：http://wwf.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rdp.hnqzz.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pwz.sufxvd.cn


<!-- 参考信息 -->