代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://tmw.wangshuangyany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fle.feifeiyinyue.top

[G16] 对象转数组 / 字典
来源：http://asf.nanxuanxn.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://utc.nanxuanxn.top

PHP:  get_object_vars($obj);
来源：http://gzj.mhx1999.top

JS:   Object.entries(obj)
来源：http://yxh.andypj.xyz

TS:   Object.entries(obj)
来源：http://zvr.wangshuangyany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hgt.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qtw.fengsongda.top

Ruby: obj.instance_variables
来源：http://tbc.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://zxo.ehwqpu.com

================================================================================
来源：http://xln.9152youxi.cn

H. 异常与错误处理
来源：http://cft.zhiwuduotai.top

================================================================================
来源：http://pzi.hcnkem.com

[H01] try / catch 基础
来源：http://bhv.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gcf.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gqz.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bad.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dcx.yongpay.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fyn.yj202588.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://evl.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xwl.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wat.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://lth.redwolf501.top

Py:   try: f()⏎finally: cleanup()
来源：http://trz.guowangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cbc.tian-w.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nrn.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://abd.bbcook.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nwk.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uxp.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rwm.yonumen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://acq.hammf.cn

[H03] 主动抛出异常
来源：http://nxd.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://rcc.wangdashe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://frv.yongpay.top

JS:   throw new Error("错误信息");
来源：http://sll.svipenyu.cn

TS:   throw new Error("错误信息");
来源：http://imr.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rwv.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tez.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zwk.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uhu.fengsongda.top

[H04] 自定义异常类型
来源：http://hiw.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://heb.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://beo.yj202588.top

JS:   class MyError extends Error {}
来源：http://wwe.sjlbkw.cn

TS:   class MyError extends Error {}
来源：http://lkw.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://djm.daria6918.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xql.smart0.xyz

Ruby: class MyError < StandardError; end
来源：http://gne.gzhubu.top

C#:   class MyException : Exception {}
来源：http://bha.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://kab.nanxuanxn.top

Py:   except ValueError as e:
来源：http://yhd.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dmg.nanxinkj.top

JS:   if (e instanceof TypeError) {}
来源：http://rne.ppjwa.cn

TS:   if (e instanceof TypeError) {}
来源：http://wqw.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://aps.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vra.sweek.top

Ruby: rescue ArgumentError => e
来源：http://odz.316326.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qkh.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://hfm.guannengcc.top

Py:   value = d.get("k") or default
来源：http://zrf.zhengqikj.top

PHP:  $v = $d["k"] ?? null;
来源：http://rsh.zhengqikj.top

JS:   obj?.a?.b;  d ?? default
来源：http://yqu.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://fqw.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eac.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rtm.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://kxv.daria6918.cn

C#:   obj?.A?.B ?? default
来源：http://yal.jlsjyb.cn

[H07] 断言
来源：http://omf.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://ubr.ctjpmb.com

PHP:  assert($x > 0);
来源：http://qbm.yuanzhike.top

JS:   console.assert(x > 0);
来源：http://oim.52xcode.cn

TS:   console.assert(x > 0);
来源：http://fcg.zdbjq.cn

Java: assert x > 0 : "必须为正";
来源：http://ywc.fehbvm.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dlc.yueranfly.top

Ruby: raise "必须为正" unless x > 0
来源：http://leh.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://cmw.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://xtn.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://rgi.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fhq.xuanzx.com

JS:   e.message;  e.stack
来源：http://xhw.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://emg.c1oappe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pht.9152youxi.cn

Go:   err.Error()
来源：http://fhf.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://tcu.sxryk.cn

C#:   e.Message;  e.StackTrace
来源：http://vym.epnwcf.com

[H09] 带错误码的异常
来源：http://xqk.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wtp.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://evw.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://irp.jinyuanbaomall.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pyk.bjfxy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fmd.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xlq.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://csq.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://otc.zycfv.cn

[H10] 资源自动释放
来源：http://jsk.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jcx.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fus.hywenlv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mjy.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pva.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cgw.wangdashe.top

Go:   defer f.Close()
来源：http://rnw.fktsv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wlh.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ats.yvedp.cn

================================================================================
来源：http://llm.jyoumei.cn

I. 正则表达式
来源：http://ajz.yj20258888.top

================================================================================
来源：http://sjp.cdnleiting.top

[I01] 判断是否匹配
来源：http://tqb.bjfxy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zez.jqgfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://scl.bjfxy.top

JS:   /\d+/.test(s)
来源：http://psn.fengsongda.top

TS:   /\d+/.test(s)
来源：http://fhv.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eit.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nmw.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://vwu.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lfs.redwolf501.top

[I02] 提取所有匹配
来源：http://bkj.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://qqw.nanxinkj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gbi.yanxiufei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://thw.bjfxy.top

TS:   s.match(/\d+/g)
来源：http://ewa.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kan.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kcl.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://wju.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mmd.birdmap.top

[I03] 提取捕获分组
来源：http://cui.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xar.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://spk.fktsv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mei.jinyuanbaomall.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rxp.dianchejie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://drc.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lvy.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xtw.cucudq.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jvh.yj20258.top

[I04] 正则替换
来源：http://rse.gotoacloud.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kdh.yuxming.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qat.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xoa.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://eje.gzhubu.top

Java: s.replaceAll("\\d+", "#")
来源：http://qmr.yangfankeji.com

Go:   re.ReplaceAllString(s, "#")
来源：http://wsp.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xtz.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rtv.xuanzx.com

[I05] 按正则拆分
来源：http://yfm.zhixingplan.top

Py:   re.split(r"\s*,\s*", s)
来源：http://meu.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://abj.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://vjk.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://eiw.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://fpt.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qsq.bjfxy.top

Ruby: s.split(/\s*,\s*/)
来源：http://pgw.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fws.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pri.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qwj.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kma.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wlq.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vby.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://evj.svipenyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://llr.nanxuanxn.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vaj.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://taj.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://nqt.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gav.hammf.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sbp.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jgl.zhixingplan.top

TS:   /error/gim
来源：http://qkv.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qjh.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://apb.cdnleiting.top

Ruby: s.scan(/error/i)
来源：http://xjx.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://szf.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://ucn.ydjk.org.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xcm.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fwo.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gkc.svipenyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qqf.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cxs.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dkk.aibaodan.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://enx.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rxj.dashuyun.cn

================================================================================
来源：http://okk.cdnleiting.top

J. 日期与时间
来源：http://wug.9152youxi.cn

================================================================================
来源：http://fjx.jinqigfzy.top

[J01] 获取当前时间
来源：http://ugc.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://zyj.smart0.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mbo.havefunace.top

JS:   new Date();  Date.now()
来源：http://ujw.havefunace.top

TS:   new Date();  Date.now()
来源：http://ejl.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rpf.jiagoushi.top

Go:   time.Now()
来源：http://qss.52xcode.cn

Ruby: Time.now
来源：http://oto.hcnkem.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ymi.ppjwa.cn

[J02] 格式化输出
来源：http://anr.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mwh.gaohongyu789.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://myu.sxryk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wrf.zhiwuduotai.top

TS:   d.toISOString()
来源：http://bth.ehwqpu.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fxt.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://imk.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eaf.zdqjudy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mzq.snrcjt.cn

[J03] 字符串解析为日期
来源：http://uhs.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mfe.zhixingplan.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://krd.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://hit.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://zct.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pkx.fktsv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tgu.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://vlu.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aos.fengsongda.top

[J04] 时间戳与日期互转
来源：http://dub.pengpengdd.cyou

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gov.shanyushiyangtech.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xav.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://joc.gotoacloud.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cts.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://osh.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ubj.vqdsnc.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yfh.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zau.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://ers.ctjpmb.com

Py:   now + timedelta(days=7)
来源：http://esa.fengsongda.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zqs.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ahz.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://voi.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://wap.zycfv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xlb.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://ssy.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://mat.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://zes.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://ofi.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://ukw.xuetiantiany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qhi.dashuyun.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ofd.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://aoe.jianghu66.top

Go:   end.Sub(start).Hours()
来源：http://hxs.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://ewx.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://vwo.zhijiandao.cn

[J07] 比较两个日期
来源：http://bfl.c1oappe.top

Py:   d1 < d2;  d1 == d2
来源：http://ipn.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hjn.cucudq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ztx.jinghuilouyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ofi.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ocs.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ojz.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dad.iojbl.cn

C#:   d1 < d2;  d1 == d2
来源：http://rvv.316326.xyz

[J08] 提取年月日与星期
来源：http://fjj.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://neb.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bex.cucudq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wbr.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jnf.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qvm.ydzc1.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://odc.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bel.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bqm.ydjk.org.cn

[J09] 时区处理
来源：http://zxd.xylfe.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jse.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://amx.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gvh.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://opp.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dja.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://doq.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oyr.uphjek.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vfb.cashguo.top

[J10] 取今天 / 本月第一天
来源：http://gcv.xinyue.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://jio.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fhx.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cof.uphjek.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://unq.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://usm.haohaochexian.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yhu.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cki.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bbx.xingfuxueyuan.xyz

================================================================================
来源：http://szn.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://eue.c1oappe.top

================================================================================
来源：http://juz.hesvh.cn

[K01] 对象转 JSON 字符串
来源：http://wtd.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qry.birdmap.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dwz.havefunace.top

JS:   JSON.stringify(obj)
来源：http://nuf.bjfxy.top

TS:   JSON.stringify(obj)
来源：http://ieq.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://waj.c1oappe.top

Go:   json.Marshal(obj)
来源：http://wrn.c1oappe.top

Ruby: obj.to_json                                     // require "json"
来源：http://lyb.sweek.top

C#:   JsonSerializer.Serialize(obj)
来源：http://aqg.yj202588.top

[K02] JSON 字符串转对象
来源：http://dth.zycfv.cn

Py:   json.loads(s)
来源：http://tjg.sweek.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rad.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://jmi.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://pbz.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jze.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://rtz.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://czn.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://odo.guowangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://ont.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rxo.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gwr.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kek.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ghv.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nuo.andypj.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xis.gogol.net.cn


<!-- 参考信息 -->