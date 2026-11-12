代发 wailian999

PHP:  get_object_vars($obj);
来源：http://png.hywenlv.cn

JS:   Object.entries(obj)
来源：http://npo.iojbl.cn

TS:   Object.entries(obj)
来源：http://bjm.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mlt.cheryme.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rky.havefunace.top

Ruby: obj.instance_variables
来源：http://ksy.chenlongwang.top

C#:   // 用反射或 System.Text.Json
来源：http://ytm.shanyushiyangtech.top

================================================================================
来源：http://lbu.chenzaomai.com

H. 异常与错误处理
来源：http://boy.chenjidiqi.icu

================================================================================
来源：http://tkh.jinyuanbaomall.cn

[H01] try / catch 基础
来源：http://usl.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uxc.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gst.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://csn.smart0.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fto.zycfv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://haf.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hsh.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cit.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qgn.aizwys.cn

[H02] finally / ensure 收尾
来源：http://hbf.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://jic.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://owb.nanxuanxn.top

JS:   try { f(); } finally { cleanup(); }
来源：http://izv.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iez.birdmap.top

Java: try { f(); } finally { cleanup(); }
来源：http://pxb.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gwz.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lkf.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://szs.fehbvm.com

[H03] 主动抛出异常
来源：http://til.aibaodan.cn

Py:   raise ValueError("错误信息")
来源：http://oys.wangdashe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ryc.ehwqpu.com

JS:   throw new Error("错误信息");
来源：http://pxc.cqqwz.cn

TS:   throw new Error("错误信息");
来源：http://vja.316326.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://buh.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mrp.epnwcf.com

Ruby: raise ArgumentError, "错误信息"
来源：http://vtz.ctjpmb.com

C#:   throw new ArgumentException("错误信息");
来源：http://kac.sysykeji.top

[H04] 自定义异常类型
来源：http://bvh.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://elj.jianghu66.top

PHP:  class MyError extends RuntimeException {}
来源：http://cko.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://wkv.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://xsg.tanke756.top

Java: class MyException extends RuntimeException {}
来源：http://fxo.vehdjk.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ciz.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://rby.zhongyouzk.top

C#:   class MyException : Exception {}
来源：http://ioo.zhengqikj.top

[H05] 捕获特定类型
来源：http://ggb.chenlongwang.top

Py:   except ValueError as e:
来源：http://enf.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eil.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://mai.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://yrj.gaohongyu789.top

Java: catch (IOException | SQLException e) {}
来源：http://pmj.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oip.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://nom.daxiang520.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hnc.zhaomingkeji.xyz

[H06] 可选值 / 空值安全访问
来源：http://cku.shanyushiyangkeji.top

Py:   value = d.get("k") or default
来源：http://idf.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xtb.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mfk.cheryme.top

TS:   obj?.a?.b;  d ?? default
来源：http://pzi.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dhc.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wyq.hammf.cn

Ruby: d&.dig(:a, :b)
来源：http://rsp.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://oqd.xziqi.cn

[H07] 断言
来源：http://lit.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://gvk.xuanzx.com

PHP:  assert($x > 0);
来源：http://ezt.redwolf501.top

JS:   console.assert(x > 0);
来源：http://ytz.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://fgo.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://mel.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gsf.yj20258.top

Ruby: raise "必须为正" unless x > 0
来源：http://wlc.yuanzhike.top

C#:   Debug.Assert(x > 0);
来源：http://eof.gzhubu.top

[H08] 获取错误信息与堆栈
来源：http://umi.jiagoushi.top

Py:   str(e);  traceback.format_exc()
来源：http://pmp.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://okq.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://hbp.pengpengdd.cyou

TS:   e instanceof Error ? e.message : String(e)
来源：http://rzs.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jbu.cucudq.cn

Go:   err.Error()
来源：http://qdt.jiagoushi.top

Ruby: e.message;  e.backtrace
来源：http://grg.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://ygu.xylfe.cn

[H09] 带错误码的异常
来源：http://qjj.yueranfly.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qrt.jlsjyb.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lzo.cheryme.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zcf.yj20258888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cbg.guannengcc.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nxh.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tfx.jyoumei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://aou.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jth.gogol.net.cn

[H10] 资源自动释放
来源：http://obb.yj20258888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jct.andypj.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zrq.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://abr.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mfk.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ezm.yvedp.cn

Go:   defer f.Close()
来源：http://fly.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cwk.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ifr.zycfv.cn

================================================================================
来源：http://euu.zhixingplan.top

I. 正则表达式
来源：http://eyg.hammf.cn

================================================================================
来源：http://gzz.zhijiandao.cn

[I01] 判断是否匹配
来源：http://bfv.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wgv.epnwcf.com

PHP:  preg_match('/\d+/', $s);
来源：http://qrt.fengsongda.top

JS:   /\d+/.test(s)
来源：http://cgs.nanxuanxn.top

TS:   /\d+/.test(s)
来源：http://axw.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uid.smart0.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zyo.jlsjyb.cn

Ruby: s.match?(/\d+/)
来源：http://dge.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fqm.shzxlz.cn

[I02] 提取所有匹配
来源：http://quu.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://gkc.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://phk.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xhh.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://pol.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://umk.hammf.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tnk.shanyushiyangtech.top

Ruby: s.scan(/\d+/)
来源：http://ngd.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xnp.gzhubu.top

[I03] 提取捕获分组
来源：http://skt.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wvc.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fkv.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gkp.daxiang520.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://snu.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://igr.sxryk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://czn.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jzv.epnwcf.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gbc.ydjk.org.cn

[I04] 正则替换
来源：http://jvs.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://eyd.nanxuanxn.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ufk.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xrk.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://vxm.ydjk.org.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jrl.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://hxz.jqgufenzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wzo.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yrm.jianghu66.top

[I05] 按正则拆分
来源：http://ykc.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://skr.hcnkem.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wzj.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://bgo.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://dpf.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://slj.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://izd.tianlin.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://zhq.hnxiangtu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xbh.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wbi.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://evu.fzhhl.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cqa.hywenlv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hma.nwbrower.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tku.andypj.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kno.guowangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tix.yfazqb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dvb.hammf.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://txc.shanyushiyangtech.top

[I07] 忽略大小写与多行模式
来源：http://idk.nanxuanxn.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xun.fzhhl.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eqm.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mih.yuanzhike.top

TS:   /error/gim
来源：http://nph.9152youxi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bxj.yfazqb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zsw.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://xpj.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bdt.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://pkb.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vhp.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://toq.zycfv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nuc.cashguo.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vwh.tianlin.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://rft.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tac.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qim.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ejt.gogol.net.cn

================================================================================
来源：http://hcd.redwolf501.top

J. 日期与时间
来源：http://olf.jlsjyb.cn

================================================================================
来源：http://lys.jinqigfzy.top

[J01] 获取当前时间
来源：http://jex.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qmn.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://glo.pycfn.com

JS:   new Date();  Date.now()
来源：http://tzr.havefunace.top

TS:   new Date();  Date.now()
来源：http://jmy.sufxvd.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dpa.hongshengwenyu.top

Go:   time.Now()
来源：http://xic.hcnkem.com

Ruby: Time.now
来源：http://rpn.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zbr.xingfuxueyuan.xyz

[J02] 格式化输出
来源：http://agg.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qap.gogol.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jzg.yueranfly.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://inx.yanxiufei.cn

TS:   d.toISOString()
来源：http://ggp.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jkz.aibaodan.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://liv.zycfv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qwk.aizwys.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://suu.guannengcc.top

[J03] 字符串解析为日期
来源：http://beu.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ney.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lnu.jqgfzy.top

JS:   new Date("2024-01-02")
来源：http://rvm.cashguo.top

TS:   new Date("2024-01-02")
来源：http://avj.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mig.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vft.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://yvf.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://avc.cheryme.top

[J04] 时间戳与日期互转
来源：http://opm.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rxh.hesvh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://thx.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rbb.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yjd.jiagoushi.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uau.yongpay.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vbk.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dmd.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aez.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://snq.xuanzx.com

Py:   now + timedelta(days=7)
来源：http://iih.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mjb.chenzaomai.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xyd.zhaomingkeji.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nlz.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://nrx.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zpu.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://bki.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://wnr.vqdsnc.cn

[J06] 计算两时间之差
来源：http://zym.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://gea.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://sip.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ioo.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rbu.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sez.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://rmz.snrcjt.cn

Ruby: end - start                 # 返回秒数
来源：http://tkj.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://rei.sjlbkw.cn

[J07] 比较两个日期
来源：http://qnu.gaohongyu789.top

Py:   d1 < d2;  d1 == d2
来源：http://kwk.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ssb.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fkt.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://wmj.bjfxy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qew.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sjc.mhx1999.top

Ruby: d1 < d2;  d1 == d2
来源：http://mzi.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://kbd.zdbjq.cn

[J08] 提取年月日与星期
来源：http://xmk.quarkkingdee.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://twy.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://usi.daria6918.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sky.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jxw.feifeiyinyue.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rtz.feifeiyinyue.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ajk.ctjpmb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vom.jqgfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cvr.shuidangran.top

[J09] 时区处理
来源：http://rai.sysykeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mlr.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mww.sysykeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hbg.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yub.hywenlv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jmy.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wfa.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ahd.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://clj.fktsv.cn

[J10] 取今天 / 本月第一天
来源：http://tbd.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://yqb.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wkc.zhiwuduotai.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ekr.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://afh.birdmap.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hgo.cheryme.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bdu.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fag.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ttc.nanxuanxn.top

================================================================================
来源：http://bsc.fanxiaobao.xyz

K. JSON 与序列化
来源：http://bem.guannengcc.top

================================================================================
来源：http://fyx.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://sre.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jik.wangdashe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://afm.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://tfm.xuanzx.com

TS:   JSON.stringify(obj)
来源：http://ree.shuidangran.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aou.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://zwz.hnqzz.top

Ruby: obj.to_json                                     // require "json"
来源：http://pfq.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jpa.yvedp.cn

[K02] JSON 字符串转对象
来源：http://dzx.shzxlz.cn

Py:   json.loads(s)
来源：http://lnr.jinghuilouyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nbv.yangfankeji.com

JS:   JSON.parse(s)
来源：http://apb.havefunace.top

TS:   JSON.parse(s)
来源：http://dnn.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mfh.yuxming.cn

Go:   json.Unmarshal(data, &v)
来源：http://nzl.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://lfi.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cet.svipenyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://dri.fehbvm.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ydg.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wko.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://dzh.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://dhu.smart0.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://idw.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uwu.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://vlr.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nda.xylfe.cn

[K04] 读取 JSON 文件
来源：http://boa.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lde.yanxiufei.cn


<!-- 参考信息 -->