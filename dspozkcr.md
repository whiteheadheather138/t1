代发 wailian999

PHP:  get_object_vars($obj);
来源：http://bvg.yuxming.cn

JS:   Object.entries(obj)
来源：http://han.tian-w.cn

TS:   Object.entries(obj)
来源：http://zhm.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fdy.jyoumei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vxf.yfazqb.com

Ruby: obj.instance_variables
来源：http://xku.pycfn.com

C#:   // 用反射或 System.Text.Json
来源：http://jci.hnqzz.top

================================================================================
来源：http://jav.nanxinkj.top

H. 异常与错误处理
来源：http://uux.yueranfly.top

================================================================================
来源：http://ktz.sufxvd.cn

[H01] try / catch 基础
来源：http://lye.cdnleiting.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jjx.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://obv.snrcjt.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lui.52xcode.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qbn.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dom.cqqwz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cvi.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lmq.tianlin.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hoj.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://ree.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qka.andypj.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://aal.pengpengdd.cyou

JS:   try { f(); } finally { cleanup(); }
来源：http://ivu.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://exy.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ynv.xylfe.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mek.birdmap.top

Ruby: begin; f; ensure; cleanup; end
来源：http://klk.quarkkingdee.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dmd.iojbl.cn

[H03] 主动抛出异常
来源：http://wnl.jiagoushi.top

Py:   raise ValueError("错误信息")
来源：http://lkg.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hgz.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://ubh.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://uib.9152youxi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uvf.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lss.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yak.andypj.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://adh.guannengcc.top

[H04] 自定义异常类型
来源：http://mcz.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://eyv.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://pfz.xinyue.icu

JS:   class MyError extends Error {}
来源：http://agr.iojbl.cn

TS:   class MyError extends Error {}
来源：http://kqx.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://zss.shanyushiyangtech.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pgc.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://rvm.dianchejie.cn

C#:   class MyException : Exception {}
来源：http://inb.c1oappe.top

[H05] 捕获特定类型
来源：http://woz.hnqzz.top

Py:   except ValueError as e:
来源：http://sez.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xvj.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://nom.hfpthk.cn

TS:   if (e instanceof TypeError) {}
来源：http://nyr.pengpengdd.cyou

Java: catch (IOException | SQLException e) {}
来源：http://xlv.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dii.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://quw.yfazqb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rys.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://jol.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://tfg.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://won.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://otl.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://uyg.gaohongyu789.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uye.iojbl.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jiu.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://lhm.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://ejr.jinqigufen.top

[H07] 断言
来源：http://zky.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://tno.zhaomingkeji.xyz

PHP:  assert($x > 0);
来源：http://tdu.iojbl.cn

JS:   console.assert(x > 0);
来源：http://isw.jiagoushi.top

TS:   console.assert(x > 0);
来源：http://icy.bjfxy.top

Java: assert x > 0 : "必须为正";
来源：http://cqq.yanxiufei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tfc.ppjwa.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wyv.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://mst.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://gsr.gotoacloud.top

Py:   str(e);  traceback.format_exc()
来源：http://bcr.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://atm.yj202588.top

JS:   e.message;  e.stack
来源：http://qrd.gotoacloud.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://eoi.yonumen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://eaw.jianghu66.top

Go:   err.Error()
来源：http://gqy.jianghu66.top

Ruby: e.message;  e.backtrace
来源：http://zrs.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://mpt.bjfxy.top

[H09] 带错误码的异常
来源：http://wye.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tun.cheryme.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lzo.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tfy.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cpr.guannengcc.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uto.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zoe.xuanzx.com

Ruby: raise MyError.new("fail", 500)
来源：http://jxs.aibaodan.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nfh.9152youxi.cn

[H10] 资源自动释放
来源：http://xms.0kj1m.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lrg.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nbo.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zka.ybcxt.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zdd.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jak.hfpthk.cn

Go:   defer f.Close()
来源：http://clg.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fwo.fanxiaobao.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hvc.zhaomingkeji.xyz

================================================================================
来源：http://nhn.cucudq.cn

I. 正则表达式
来源：http://vtn.xuanzx.com

================================================================================
来源：http://fxs.gaohongyu789.top

[I01] 判断是否匹配
来源：http://ykm.hnqzz.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eph.sweek.top

PHP:  preg_match('/\d+/', $s);
来源：http://pgg.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://ndn.jianghu66.top

TS:   /\d+/.test(s)
来源：http://rms.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fpv.zycfv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qii.fengsongda.top

Ruby: s.match?(/\d+/)
来源：http://abm.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ryn.aizwys.cn

[I02] 提取所有匹配
来源：http://abq.jqgfzy.top

Py:   re.findall(r"\d+", s)
来源：http://cjd.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tzv.yueranfly.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rhf.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://mch.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nps.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pzq.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://lrh.yvedp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zjm.aizwys.cn

[I03] 提取捕获分组
来源：http://ssj.guannengcc.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oju.xinyue.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://itf.shangyingyoupin.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zky.dianchejie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vng.sysykeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fvm.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ilj.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lms.hcnkem.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://owe.redwolf501.top

[I04] 正则替换
来源：http://iwg.hongshengwenyu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wgl.hongshengwenyu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kiw.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://elt.xylfe.cn

TS:   s.replace(/\d+/g, "#")
来源：http://glp.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://hjs.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mau.hesvh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vsh.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pxy.hysaishi.cn

[I05] 按正则拆分
来源：http://zmo.sjlbkw.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://obz.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zdq.vqdsnc.cn

JS:   s.split(/\s*,\s*/)
来源：http://ayg.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://wez.hfpthk.cn

Java: s.split("\\s*,\\s*")
来源：http://cci.zhiwuduotai.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gwx.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://wuo.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nch.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xdh.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ezh.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zyf.vehdjk.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iwo.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yju.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mhj.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://inp.yonumen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gzg.yvedp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://teg.daria6918.cn

[I07] 忽略大小写与多行模式
来源：http://sqk.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gnt.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vyg.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rud.hcnkem.com

TS:   /error/gim
来源：http://nkt.yuxming.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vur.xylfe.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gbc.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://rax.smart0.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vby.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://zco.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uet.zhengqikj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hmp.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fhi.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://usa.gogol.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eky.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bho.fanxiaobao.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eqi.zhijiandao.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ota.gzhubu.top

================================================================================
来源：http://rcw.zdbjq.cn

J. 日期与时间
来源：http://urb.jqgfzy.top

================================================================================
来源：http://hvw.chenlongwang.top

[J01] 获取当前时间
来源：http://gso.zycfv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sju.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rmu.tanke756.top

JS:   new Date();  Date.now()
来源：http://hir.yj202588.top

TS:   new Date();  Date.now()
来源：http://oln.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ene.hywenlv.cn

Go:   time.Now()
来源：http://lkx.cucudq.cn

Ruby: Time.now
来源：http://skg.wangshuangyany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sah.shangyingyoupin.top

[J02] 格式化输出
来源：http://jxd.kuanghao11.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zww.bbcook.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://shl.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://stw.tarul.cn

TS:   d.toISOString()
来源：http://cnh.ywan-chungtsiang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wha.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vfr.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hmp.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nvh.xylfe.cn

[J03] 字符串解析为日期
来源：http://ysr.sysykeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pvw.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xeb.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://aud.sxryk.cn

TS:   new Date("2024-01-02")
来源：http://ntg.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://bgd.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://anc.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://ogy.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yez.xylfe.cn

[J04] 时间戳与日期互转
来源：http://mai.xziqi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yem.zdbjq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jzg.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://niq.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jjq.fehbvm.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nav.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ujl.nanxinkj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tkf.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qqs.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://edd.snrcjt.cn

Py:   now + timedelta(days=7)
来源：http://exj.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://evb.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://euk.yfazqb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zuf.bjfxy.top

Java: LocalDate.now().plusDays(7)
来源：http://bqc.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://miq.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://oqm.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://zjb.jlsjyb.cn

[J06] 计算两时间之差
来源：http://jvf.ywan-chungtsiang.top

Py:   (end - start).total_seconds()
来源：http://jws.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://jpn.svipenyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hxq.nwbrower.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://coo.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://bad.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://axs.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://qhc.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://psu.shangyingyoupin.top

[J07] 比较两个日期
来源：http://suk.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://iyq.jiagoushi.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dsh.shuidangran.top

JS:   d1.getTime() < d2.getTime()
来源：http://peg.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vpg.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eos.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://osf.epnwcf.com

Ruby: d1 < d2;  d1 == d2
来源：http://qdz.shuidangran.top

C#:   d1 < d2;  d1 == d2
来源：http://qos.52xcode.cn

[J08] 提取年月日与星期
来源：http://qfm.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pgn.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iik.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ldm.hysaishi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nfi.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wvn.yj20258.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://adx.nwbrower.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zly.yj20258.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fnx.zhijiandao.cn

[J09] 时区处理
来源：http://tvu.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vki.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ezw.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fmj.iojbl.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://juc.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xed.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yqn.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nhp.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pun.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://bzf.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tyh.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yzd.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ndc.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wuz.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zdk.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://orz.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kzh.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vuk.hywenlv.cn

================================================================================
来源：http://bbw.ybcxt.top

K. JSON 与序列化
来源：http://rix.9152youxi.cn

================================================================================
来源：http://ipd.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://xgz.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://alo.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hdu.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://wte.wangshuangyany.cn

TS:   JSON.stringify(obj)
来源：http://xvp.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bdv.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://hua.dianchejie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pqs.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gth.yuxming.cn

[K02] JSON 字符串转对象
来源：http://eaz.bbcook.cn

Py:   json.loads(s)
来源：http://orf.ppjwa.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qzy.fengsongda.top

JS:   JSON.parse(s)
来源：http://txv.bbcook.cn

TS:   JSON.parse(s)
来源：http://rtt.jlsjyb.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://glo.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://uwp.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://qut.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vtd.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://mwz.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gpf.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://olb.fanxiaobao.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://mec.zhijiandao.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ogs.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gby.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mob.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://lab.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ywy.shuidangran.top

[K04] 读取 JSON 文件
来源：http://gic.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vxg.andypj.xyz


<!-- 参考信息 -->