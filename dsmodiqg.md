代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eey.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://atl.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://uza.pengpengdd.cyou

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wsi.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://sqq.shuidangran.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rfq.pycfn.com

[G16] 对象转数组 / 字典
来源：http://yyi.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nem.aizwys.cn

PHP:  get_object_vars($obj);
来源：http://egl.chenzaomai.com

JS:   Object.entries(obj)
来源：http://ftn.ybcxt.top

TS:   Object.entries(obj)
来源：http://hrl.tarul.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hjf.meibo888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://utz.zhongyouzk.top

Ruby: obj.instance_variables
来源：http://kmd.tarul.cn

C#:   // 用反射或 System.Text.Json
来源：http://hrp.316326.xyz

================================================================================
来源：http://yug.hcnkem.com

H. 异常与错误处理
来源：http://rxw.jqgfzy.top

================================================================================
来源：http://ttg.zhijiandao.cn

[H01] try / catch 基础
来源：http://trb.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dsy.52xcode.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pbp.tarul.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://quj.tarul.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fml.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dnv.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pgb.snrcjt.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mmm.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jkb.c1oappe.top

[H02] finally / ensure 收尾
来源：http://wij.yfazqb.com

Py:   try: f()⏎finally: cleanup()
来源：http://uvo.c1oappe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gvo.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vdc.zhixingplan.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gtl.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://aok.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ent.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jkg.tianlin.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://tar.fzhhl.top

[H03] 主动抛出异常
来源：http://pca.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://rpo.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hbp.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://jlk.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://gxk.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://epo.daria6918.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://efx.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zhj.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://kha.c1oappe.top

[H04] 自定义异常类型
来源：http://lde.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://mei.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://okq.pengpengdd.cyou

JS:   class MyError extends Error {}
来源：http://yim.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://lov.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://ten.jqgfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vab.jinyuanbaomall.cn

Ruby: class MyError < StandardError; end
来源：http://fqo.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://nnc.sweek.top

[H05] 捕获特定类型
来源：http://hmr.svipenyu.cn

Py:   except ValueError as e:
来源：http://aux.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://efh.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://mxv.zhengqikj.top

TS:   if (e instanceof TypeError) {}
来源：http://rsp.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://oic.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vyp.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://zch.jyoumei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qru.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://qkf.fehbvm.com

Py:   value = d.get("k") or default
来源：http://qbf.andypj.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://hfh.sweek.top

JS:   obj?.a?.b;  d ?? default
来源：http://yio.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://lse.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://huq.hammf.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://owl.yangfankeji.com

Ruby: d&.dig(:a, :b)
来源：http://hup.jinyuanbaomall.cn

C#:   obj?.A?.B ?? default
来源：http://vgp.epnwcf.com

[H07] 断言
来源：http://uam.birdmap.top

Py:   assert x > 0, "必须为正"
来源：http://ezf.shuidangran.top

PHP:  assert($x > 0);
来源：http://lzk.cashguo.top

JS:   console.assert(x > 0);
来源：http://equ.daxiang520.top

TS:   console.assert(x > 0);
来源：http://bsb.ehwqpu.com

Java: assert x > 0 : "必须为正";
来源：http://all.ybcxt.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://idl.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://enq.gzhubu.top

C#:   Debug.Assert(x > 0);
来源：http://cti.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://bld.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://ife.bbcook.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xfn.zhixingplan.top

JS:   e.message;  e.stack
来源：http://spz.hesvh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lkc.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://tvo.hywenlv.cn

Go:   err.Error()
来源：http://ywp.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://gtd.fzhhl.top

C#:   e.Message;  e.StackTrace
来源：http://gou.epnwcf.com

[H09] 带错误码的异常
来源：http://ikg.aizwys.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bsa.epnwcf.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://plb.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zuq.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qjb.nanxuanxn.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vve.mhx1999.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oui.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://mze.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://cne.yuxming.cn

[H10] 资源自动释放
来源：http://uhh.yueranfly.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lei.bjfxy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gwq.yj20258.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://atb.ybcxt.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://twz.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yfl.xylfe.cn

Go:   defer f.Close()
来源：http://ikq.dianchejie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tjx.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hva.andypj.xyz

================================================================================
来源：http://jzm.xinyue.icu

I. 正则表达式
来源：http://maz.yj20258.top

================================================================================
来源：http://cal.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://jjv.daxiang520.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://klr.0kj1m.cn

PHP:  preg_match('/\d+/', $s);
来源：http://iho.xylfe.cn

JS:   /\d+/.test(s)
来源：http://alc.sxryk.cn

TS:   /\d+/.test(s)
来源：http://xtz.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://anu.andypj.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yqr.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://rsi.gzhubu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://idz.sxryk.cn

[I02] 提取所有匹配
来源：http://iok.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://aao.nwbrower.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nwi.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mij.yongpay.top

TS:   s.match(/\d+/g)
来源：http://ser.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nyf.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yha.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://ywl.bjfxy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qdp.zycfv.cn

[I03] 提取捕获分组
来源：http://bro.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kwm.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mvz.wangshuangyany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://omy.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jmi.snrcjt.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tua.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gkb.52xcode.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lyk.andypj.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hcr.nanxuanxn.top

[I04] 正则替换
来源：http://zoc.guannengcc.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zjb.yongpay.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://slw.yonumen.top

JS:   s.replace(/\d+/g, "#")
来源：http://eue.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vps.shangyingyoupin.top

Java: s.replaceAll("\\d+", "#")
来源：http://ype.hongshengwenyu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ntb.hongshengwenyu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vyr.zhengqikj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://njr.zhijiandao.cn

[I05] 按正则拆分
来源：http://kue.jinqigufen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rmt.hnxiangtu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://axm.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://ovj.yuxming.cn

TS:   s.split(/\s*,\s*/)
来源：http://zcw.sysykeji.top

Java: s.split("\\s*,\\s*")
来源：http://ixz.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hsm.xuetiantiany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hyz.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nyb.ehwqpu.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kut.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qnl.tianlin.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nzp.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ego.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ros.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pev.fanxiaobao.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://drc.nwbrower.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eej.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tnw.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://ext.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zgf.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kdb.feifeiyinyue.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fka.hongshengwenyu.top

TS:   /error/gim
来源：http://yfu.svipenyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rzg.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dok.shzxlz.cn

Ruby: s.scan(/error/i)
来源：http://yoh.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pvs.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://bvg.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dld.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bzh.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ufm.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jkh.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://qlo.sjlbkw.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://emg.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ekx.cashguo.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uwd.bbcook.cn

================================================================================
来源：http://ngs.birdmap.top

J. 日期与时间
来源：http://ndj.daxiang520.top

================================================================================
来源：http://wde.jinqigfzy.top

[J01] 获取当前时间
来源：http://sae.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://led.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hfd.yj20258.top

JS:   new Date();  Date.now()
来源：http://bls.quarkkingdee.top

TS:   new Date();  Date.now()
来源：http://wxi.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sfc.yfazqb.com

Go:   time.Now()
来源：http://exv.xziqi.cn

Ruby: Time.now
来源：http://twm.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ndp.daria6918.cn

[J02] 格式化输出
来源：http://ama.xinyue.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lfb.zhoulong.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jim.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kes.jyoumei.cn

TS:   d.toISOString()
来源：http://pvg.meibo888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://arm.gotoacloud.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ufy.hnxiangtu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ubt.jqgufenzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yxg.sxryk.cn

[J03] 字符串解析为日期
来源：http://lna.aibaodan.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ldo.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bxz.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://jwx.havefunace.top

TS:   new Date("2024-01-02")
来源：http://vpi.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://bzg.bjfxy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xlc.sxryk.cn

Ruby: Date.parse("2024-01-02")
来源：http://mhs.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uja.cucudq.cn

[J04] 时间戳与日期互转
来源：http://phj.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ewq.shanyushiyangtech.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nhh.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ibt.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nxo.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zug.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gtm.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fkq.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fft.pengpengdd.cyou

[J05] 时间加减（加 7 天）
来源：http://quc.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://zxk.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://lqu.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iab.smart0.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xrl.jqgufenzy.top

Java: LocalDate.now().plusDays(7)
来源：http://mbq.pengpengdd.cyou

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fax.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://ecb.birdmap.top

C#:   DateTime.Now.AddDays(7)
来源：http://mow.tanke756.top

[J06] 计算两时间之差
来源：http://jjq.sweek.top

Py:   (end - start).total_seconds()
来源：http://mbl.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://gwh.cdnleiting.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cex.havefunace.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lim.sxryk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hpu.52xcode.cn

Go:   end.Sub(start).Hours()
来源：http://rmf.cqqwz.cn

Ruby: end - start                 # 返回秒数
来源：http://yda.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://orn.chenlongwang.top

[J07] 比较两个日期
来源：http://lze.fehbvm.com

Py:   d1 < d2;  d1 == d2
来源：http://lmw.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uof.shuidangran.top

JS:   d1.getTime() < d2.getTime()
来源：http://saf.sxryk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ugm.gaohongyu789.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eho.vqdsnc.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eup.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ebk.sxryk.cn

C#:   d1 < d2;  d1 == d2
来源：http://jne.nwbrower.top

[J08] 提取年月日与星期
来源：http://tos.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yoc.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ces.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ylh.tanke756.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sdh.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hsx.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nos.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ftv.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xhc.meibo888.top

[J09] 时区处理
来源：http://yuz.ehwqpu.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eon.fengsongda.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://slm.dianchejie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uhw.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tvn.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pfi.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kgt.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://scy.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rvy.bjfxy.top

[J10] 取今天 / 本月第一天
来源：http://sys.shuidangran.top

Py:   date.today();  date.today().replace(day=1)
来源：http://acn.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jzh.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ydj.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://afn.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oyl.hcnkem.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dvq.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ccl.fktsv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vze.xinyue.icu

================================================================================
来源：http://wcs.tanke756.top

K. JSON 与序列化
来源：http://fol.316326.xyz

================================================================================
来源：http://xdi.ivvv.top

[K01] 对象转 JSON 字符串
来源：http://hfg.hesvh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://npw.jianghu66.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vfz.hnxiangtu.top

JS:   JSON.stringify(obj)
来源：http://ifu.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://jbq.wangshuangyany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xpg.shuidangran.top

Go:   json.Marshal(obj)
来源：http://fmr.kuanghao11.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xgk.meibo888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ela.52xcode.cn

[K02] JSON 字符串转对象
来源：http://mzf.gotoacloud.top

Py:   json.loads(s)
来源：http://chs.ybcxt.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pis.hywenlv.cn

JS:   JSON.parse(s)
来源：http://gsl.havefunace.top

TS:   JSON.parse(s)
来源：http://smx.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jru.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://drz.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://enx.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://otg.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://luf.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uvb.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ypw.yanxiufei.cn


<!-- 参考信息 -->