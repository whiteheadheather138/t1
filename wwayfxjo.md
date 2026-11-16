代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://vfp.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qgm.jianghu66.top

[G16] 对象转数组 / 字典
来源：http://cui.ppjwa.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://adg.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://lun.xziqi.cn

JS:   Object.entries(obj)
来源：http://rih.cashguo.top

TS:   Object.entries(obj)
来源：http://yru.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ofz.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sul.xuetiantiany.cn

Ruby: obj.instance_variables
来源：http://yqe.yfazqb.com

C#:   // 用反射或 System.Text.Json
来源：http://qmz.zycfv.cn

================================================================================
来源：http://ffj.sweek.top

H. 异常与错误处理
来源：http://brz.zhixingplan.top

================================================================================
来源：http://nwg.quarkkingdee.top

[H01] try / catch 基础
来源：http://gfs.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qxj.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://thu.nanxuanxn.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qrk.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ekp.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://urx.yuxming.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dsb.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bhg.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vhs.zdqjudy.top

[H02] finally / ensure 收尾
来源：http://ngv.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://sff.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fom.ydjk.org.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://eiy.nwbrower.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nxn.jinqigfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://aoa.bjfxy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://txg.zhijiandao.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rue.zhengqikj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zls.guannengcc.top

[H03] 主动抛出异常
来源：http://isi.xziqi.cn

Py:   raise ValueError("错误信息")
来源：http://uwc.jiagoushi.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://apm.xziqi.cn

JS:   throw new Error("错误信息");
来源：http://jfu.yuxming.cn

TS:   throw new Error("错误信息");
来源：http://nqh.tanke756.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zil.zhijiandao.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qwh.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ste.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://eia.xuetiantiany.cn

[H04] 自定义异常类型
来源：http://wpd.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://gks.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bau.cqqwz.cn

JS:   class MyError extends Error {}
来源：http://bre.yonumen.top

TS:   class MyError extends Error {}
来源：http://vzg.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://won.uphjek.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tbf.hcnkem.com

Ruby: class MyError < StandardError; end
来源：http://llw.chenjidiqi.icu

C#:   class MyException : Exception {}
来源：http://bpk.nanxinkj.top

[H05] 捕获特定类型
来源：http://dib.tian-w.cn

Py:   except ValueError as e:
来源：http://qfq.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oqi.gaohongyu789.top

JS:   if (e instanceof TypeError) {}
来源：http://wvl.ywan-chungtsiang.top

TS:   if (e instanceof TypeError) {}
来源：http://oko.ywan-chungtsiang.top

Java: catch (IOException | SQLException e) {}
来源：http://wzt.svipenyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bmd.zhongyouzk.top

Ruby: rescue ArgumentError => e
来源：http://rzc.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zgm.jlsjyb.cn

[H06] 可选值 / 空值安全访问
来源：http://vae.pengpengdd.cyou

Py:   value = d.get("k") or default
来源：http://fvo.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://xya.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://udp.xziqi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qxs.hesvh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tel.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gkk.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://vng.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://fbg.meibo888.top

[H07] 断言
来源：http://abd.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://rre.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://wev.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://fhv.chenlongwang.top

TS:   console.assert(x > 0);
来源：http://exh.havefunace.top

Java: assert x > 0 : "必须为正";
来源：http://dvh.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cgv.xinyue.icu

Ruby: raise "必须为正" unless x > 0
来源：http://xrr.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://dwe.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://yop.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://vem.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vef.xinyue.icu

JS:   e.message;  e.stack
来源：http://brv.cdnleiting.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nfi.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://aab.bbcook.cn

Go:   err.Error()
来源：http://lkh.tian-w.cn

Ruby: e.message;  e.backtrace
来源：http://gzb.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://iko.sufxvd.cn

[H09] 带错误码的异常
来源：http://lfq.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uyz.xylfe.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xcf.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ead.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xfs.xuetiantiany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qxc.316326.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lgy.gaohongyu789.top

Ruby: raise MyError.new("fail", 500)
来源：http://div.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ezm.mhx1999.top

[H10] 资源自动释放
来源：http://fqx.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nqr.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kfj.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kev.yj202588.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vqt.gotoacloud.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qhu.bjfxy.top

Go:   defer f.Close()
来源：http://ujc.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bts.yvedp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ypb.shanyushiyangkeji.top

================================================================================
来源：http://mvc.hesvh.cn

I. 正则表达式
来源：http://jvg.0kj1m.cn

================================================================================
来源：http://ebs.zdqjudy.top

[I01] 判断是否匹配
来源：http://wnh.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kzk.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tgp.bjfxy.top

JS:   /\d+/.test(s)
来源：http://pfs.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://fku.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qlh.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uwi.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://ggh.jyoumei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bte.ybcxt.top

[I02] 提取所有匹配
来源：http://etw.nanxinkj.top

Py:   re.findall(r"\d+", s)
来源：http://hid.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://skw.nanxinkj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gzc.jinyuanbaomall.cn

TS:   s.match(/\d+/g)
来源：http://fgm.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://onh.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mju.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://adj.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xvi.jiagoushi.top

[I03] 提取捕获分组
来源：http://qif.guowangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lsw.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lsb.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uft.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nlo.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rfh.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qkq.chenjidiqi.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ntg.yanxiufei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wsz.guowangkeji.top

[I04] 正则替换
来源：http://cyh.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fxl.fengsongda.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xas.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sid.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://vjf.fengsongda.top

Java: s.replaceAll("\\d+", "#")
来源：http://wau.jinqigufen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ipf.yanxiufei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cxe.redwolf501.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xeo.zhixingplan.top

[I05] 按正则拆分
来源：http://qtx.chenjidiqi.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://zjn.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://orv.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://pev.zhaomingkeji.xyz

TS:   s.split(/\s*,\s*/)
来源：http://acp.sjlbkw.cn

Java: s.split("\\s*,\\s*")
来源：http://fwc.tanke756.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ucw.birdmap.top

Ruby: s.split(/\s*,\s*/)
来源：http://fti.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dji.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yxt.jinghuilouyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wny.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cds.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uvx.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kim.bjfxy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ypj.guowangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oyj.ydzc1.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xfl.jlsjyb.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yum.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://dqy.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rtr.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mlr.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wrv.aizwys.cn

TS:   /error/gim
来源：http://gvf.ydzc1.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xms.hesvh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qea.zhongyouzk.top

Ruby: s.scan(/error/i)
来源：http://vpk.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://idk.bjfxy.top

[I08] 贪婪与非贪婪匹配
来源：http://ydy.havefunace.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gyp.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nfm.zhixingplan.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wey.xingfuxueyuan.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rlr.pycfn.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://rwz.xziqi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tra.gogol.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vob.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yyv.ppjwa.cn

================================================================================
来源：http://lqz.ydzc1.top

J. 日期与时间
来源：http://nff.ppjwa.cn

================================================================================
来源：http://yzn.zhijiandao.cn

[J01] 获取当前时间
来源：http://two.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yuk.fktsv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jrn.mhx1999.top

JS:   new Date();  Date.now()
来源：http://jhn.52xcode.cn

TS:   new Date();  Date.now()
来源：http://bet.ydjk.org.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dqm.guannengcc.top

Go:   time.Now()
来源：http://ogz.cucudq.cn

Ruby: Time.now
来源：http://ucn.nwbrower.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vuo.meibo888.top

[J02] 格式化输出
来源：http://dif.jianghu66.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oiu.yj20258888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ukb.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://viq.zdqjudy.top

TS:   d.toISOString()
来源：http://pdf.shzxlz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vkt.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fsz.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://egt.wangdashe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gdj.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://lbn.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xjz.0kj1m.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mau.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://ljc.cqqwz.cn

TS:   new Date("2024-01-02")
来源：http://rpc.cqqwz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pkd.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://raa.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://qld.yueranfly.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gjg.aizwys.cn

[J04] 时间戳与日期互转
来源：http://rql.cashguo.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wdb.smart0.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wko.yj20258888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://swf.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://hig.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://goy.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iat.jlsjyb.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qkn.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nux.hnqzz.top

[J05] 时间加减（加 7 天）
来源：http://mow.xinyue.icu

Py:   now + timedelta(days=7)
来源：http://aqf.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ogk.xingfuxueyuan.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vlb.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pyi.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://zzk.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jya.yuxming.cn

Ruby: Time.now + 7 * 86400
来源：http://vat.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cuk.ydzc1.top

[J06] 计算两时间之差
来源：http://nkv.shanyushiyangtech.top

Py:   (end - start).total_seconds()
来源：http://jei.smart0.xyz

PHP:  $end->diff($start)->days;
来源：http://ida.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xnp.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oxp.cashguo.top

Java: Duration.between(start, end).toSeconds()
来源：http://zjv.sjlbkw.cn

Go:   end.Sub(start).Hours()
来源：http://hzx.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://rkd.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://ycc.tanke756.top

[J07] 比较两个日期
来源：http://apu.iojbl.cn

Py:   d1 < d2;  d1 == d2
来源：http://aao.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dmt.fktsv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://edu.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kmb.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hee.chenzaomai.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lly.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://scu.cdnleiting.top

C#:   d1 < d2;  d1 == d2
来源：http://zop.uphjek.com

[J08] 提取年月日与星期
来源：http://fhz.ehwqpu.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oyn.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ymx.sysykeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yws.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rpb.shangyingyoupin.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oya.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ruu.yonumen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hkf.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ref.aizwys.cn

[J09] 时区处理
来源：http://jve.hammf.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lhc.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qxz.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bfw.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qki.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://haq.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://edu.ywan-chungtsiang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hfc.havefunace.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pvm.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://grq.aizwys.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dlw.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rfu.cheryme.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uvl.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vmy.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pgi.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eiu.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jkx.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://esn.hysaishi.cn

================================================================================
来源：http://uos.zycfv.cn

K. JSON 与序列化
来源：http://twr.nanxuanxn.top

================================================================================
来源：http://gjd.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://rey.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fdw.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hss.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://daa.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://zys.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jqy.hesvh.cn

Go:   json.Marshal(obj)
来源：http://dau.chenlongwang.top

Ruby: obj.to_json                                     // require "json"
来源：http://rlg.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ecs.wangshuangyany.cn

[K02] JSON 字符串转对象
来源：http://lvv.zdbjq.cn

Py:   json.loads(s)
来源：http://yjy.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vtp.ivvv.top

JS:   JSON.parse(s)
来源：http://aeo.xuetiantiany.cn

TS:   JSON.parse(s)
来源：http://kyh.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://unh.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://jgg.aizwys.cn

Ruby: JSON.parse(s)
来源：http://ouy.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bup.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://aqx.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://acl.ppjwa.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pso.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fev.yongpay.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lwk.mhx1999.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gnu.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jyf.hysaishi.cn


<!-- 参考信息 -->