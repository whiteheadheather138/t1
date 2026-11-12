代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://tns.yj20258.top

Ruby: obj.instance_variables
来源：http://kec.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://hmz.hammf.cn

================================================================================
来源：http://nfz.yuanzhike.top

H. 异常与错误处理
来源：http://mwa.aibaodan.cn

================================================================================
来源：http://gad.sjlbkw.cn

[H01] try / catch 基础
来源：http://gyd.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://neq.yj202588.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rlp.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qqx.gogol.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://avf.jyoumei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tip.iojbl.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ygv.zhixingplan.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hqa.yueranfly.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://omq.xziqi.cn

[H02] finally / ensure 收尾
来源：http://ffl.hesvh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qhx.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tlk.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tdk.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://sng.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://upo.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://uzb.gaohongyu789.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xly.zhijiandao.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iap.316326.xyz

[H03] 主动抛出异常
来源：http://zbq.yanxiufei.cn

Py:   raise ValueError("错误信息")
来源：http://jfm.yueranfly.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pmz.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://gvq.chenlongwang.top

TS:   throw new Error("错误信息");
来源：http://vqw.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://jem.tian-w.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nrp.ctjpmb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://zhs.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://ctg.xylfe.cn

[H04] 自定义异常类型
来源：http://kzm.ydjk.org.cn

Py:   class MyError(Exception): pass
来源：http://imw.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fwp.vehdjk.com

JS:   class MyError extends Error {}
来源：http://rmf.cheryme.top

TS:   class MyError extends Error {}
来源：http://mru.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://yhd.yuxming.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sjs.cheryme.top

Ruby: class MyError < StandardError; end
来源：http://fiv.uphjek.com

C#:   class MyException : Exception {}
来源：http://soe.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://nmo.gotoacloud.top

Py:   except ValueError as e:
来源：http://lxa.shangyingyoupin.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nku.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://fcq.zycfv.cn

TS:   if (e instanceof TypeError) {}
来源：http://aye.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://ntw.0kj1m.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://htp.shangyingyoupin.top

Ruby: rescue ArgumentError => e
来源：http://ozz.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mgi.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://dps.shanyushiyangkeji.top

Py:   value = d.get("k") or default
来源：http://mwq.nanxuanxn.top

PHP:  $v = $d["k"] ?? null;
来源：http://sgl.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://wxy.ivvv.top

TS:   obj?.a?.b;  d ?? default
来源：http://ans.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hbs.ydjk.org.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gib.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://hce.vqdsnc.cn

C#:   obj?.A?.B ?? default
来源：http://ubs.andypj.xyz

[H07] 断言
来源：http://tgv.daxiang520.top

Py:   assert x > 0, "必须为正"
来源：http://suu.yj202588.top

PHP:  assert($x > 0);
来源：http://yft.xinyue.icu

JS:   console.assert(x > 0);
来源：http://yek.epnwcf.com

TS:   console.assert(x > 0);
来源：http://zbi.yongpay.top

Java: assert x > 0 : "必须为正";
来源：http://ala.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sth.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wrw.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://mze.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://sld.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://qqo.shanyushiyangtech.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pby.yanxiufei.cn

JS:   e.message;  e.stack
来源：http://hts.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mph.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://juc.snrcjt.cn

Go:   err.Error()
来源：http://pmh.sweek.top

Ruby: e.message;  e.backtrace
来源：http://hyk.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://dza.yueranfly.top

[H09] 带错误码的异常
来源：http://nlh.tianlin.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dhg.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://srk.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xyj.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dst.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lmg.ydzc1.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jnk.zhijiandao.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mup.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ebt.cheryme.top

[H10] 资源自动释放
来源：http://hib.sxryk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xtq.sysykeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lrj.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mwr.vqdsnc.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dal.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ijv.hywenlv.cn

Go:   defer f.Close()
来源：http://fwn.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pnk.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://exs.sufxvd.cn

================================================================================
来源：http://jsw.yanxiufei.cn

I. 正则表达式
来源：http://ajg.jinyuanbaomall.cn

================================================================================
来源：http://ldo.jqgufenzy.top

[I01] 判断是否匹配
来源：http://fvv.jlsjyb.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rpw.ywan-chungtsiang.top

PHP:  preg_match('/\d+/', $s);
来源：http://itu.shanyushiyangtech.top

JS:   /\d+/.test(s)
来源：http://tpt.hesvh.cn

TS:   /\d+/.test(s)
来源：http://gca.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://naf.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mzk.cdnleiting.top

Ruby: s.match?(/\d+/)
来源：http://rxo.cashguo.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kok.zhoulong.xyz

[I02] 提取所有匹配
来源：http://nom.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://iaf.sufxvd.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://clv.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://prp.jinghuilouyu.cn

TS:   s.match(/\d+/g)
来源：http://rck.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tvm.sweek.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bad.tarul.cn

Ruby: s.scan(/\d+/)
来源：http://cvg.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gcy.ivvv.top

[I03] 提取捕获分组
来源：http://zqt.hnqzz.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ztp.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kdt.cdnleiting.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tef.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sbi.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vmy.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hsu.sufxvd.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zao.tarul.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://njg.shangyingyoupin.top

[I04] 正则替换
来源：http://cvg.nanxuanxn.top

Py:   re.sub(r"\d+", "#", s)
来源：http://toj.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://shs.nanxinkj.top

JS:   s.replace(/\d+/g, "#")
来源：http://xab.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://yxr.nanxuanxn.top

Java: s.replaceAll("\\d+", "#")
来源：http://cuu.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wqg.yangfankeji.com

Ruby: s.gsub(/\d+/, "#")
来源：http://lok.yanxiufei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://drs.aizwys.cn

[I05] 按正则拆分
来源：http://tkd.fengsongda.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ejx.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://exw.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://lcg.ybcxt.top

TS:   s.split(/\s*,\s*/)
来源：http://cze.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://ejd.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hqn.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://htm.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gjr.tianlin.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kgb.smart0.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kab.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rdh.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zrq.xuanzx.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pjx.ehwqpu.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rxi.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://utg.zdqjudy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tfs.jyoumei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rhx.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://xzg.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qrh.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mmd.ydjk.org.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://prq.xinyue.icu

TS:   /error/gim
来源：http://sca.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lcw.daria6918.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nbv.daria6918.cn

Ruby: s.scan(/error/i)
来源：http://plg.daria6918.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://otl.fzhhl.top

[I08] 贪婪与非贪婪匹配
来源：http://uqa.fktsv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qey.aibaodan.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://esw.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://akz.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xan.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://czb.yuanzhike.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oxd.cashguo.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ctz.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cbr.meibo888.top

================================================================================
来源：http://cmq.c1oappe.top

J. 日期与时间
来源：http://bux.jqgfzy.top

================================================================================
来源：http://zfq.zdbjq.cn

[J01] 获取当前时间
来源：http://aol.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tda.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vok.smart0.xyz

JS:   new Date();  Date.now()
来源：http://pyv.316326.xyz

TS:   new Date();  Date.now()
来源：http://zul.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jva.hongshengwenyu.top

Go:   time.Now()
来源：http://uwf.aizwys.cn

Ruby: Time.now
来源：http://vux.hcnkem.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rws.dianchejie.cn

[J02] 格式化输出
来源：http://kuf.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aql.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pop.yuxming.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hun.epnwcf.com

TS:   d.toISOString()
来源：http://shf.hcnkem.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aqn.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cyo.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zec.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tav.jinyuanbaomall.cn

[J03] 字符串解析为日期
来源：http://upu.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hoy.shangyingyoupin.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oqy.yj202588.top

JS:   new Date("2024-01-02")
来源：http://pmv.shuidangran.top

TS:   new Date("2024-01-02")
来源：http://igc.jlsjyb.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vvt.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://umg.pycfn.com

Ruby: Date.parse("2024-01-02")
来源：http://qcj.cdnleiting.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bhx.daria6918.cn

[J04] 时间戳与日期互转
来源：http://ojq.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nlq.hnqzz.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wak.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://csy.wangshuangyany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://thy.zdbjq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tbr.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ibj.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xqf.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://epa.cheryme.top

[J05] 时间加减（加 7 天）
来源：http://cto.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://jdf.yj20258.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pua.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bto.hysaishi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mcl.zhiwuduotai.top

Java: LocalDate.now().plusDays(7)
来源：http://etf.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hnd.yuanzhike.top

Ruby: Time.now + 7 * 86400
来源：http://nvl.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://hwk.quarkkingdee.top

[J06] 计算两时间之差
来源：http://clz.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://rew.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://tkk.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ysj.xylfe.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kjn.fktsv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cem.birdmap.top

Go:   end.Sub(start).Hours()
来源：http://ajj.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://snu.cashguo.top

C#:   (end - start).TotalSeconds
来源：http://sxj.yanxiufei.cn

[J07] 比较两个日期
来源：http://ekz.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://fqj.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ldb.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nqv.zycfv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gwz.9152youxi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bpc.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wng.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zmv.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://gts.haohaochexian.top

[J08] 提取年月日与星期
来源：http://efy.shanyushiyangtech.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ioe.pengpengdd.cyou

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pqa.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mkw.hcnkem.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hgg.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zdy.vqdsnc.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://joh.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://teq.aibaodan.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mau.zhongyouzk.top

[J09] 时区处理
来源：http://phw.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hgx.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hwj.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tex.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lpp.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pig.havefunace.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fmd.hammf.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jka.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dph.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://xok.ivvv.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hva.xingfuxueyuan.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tnz.yongpay.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wtj.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cod.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dad.fktsv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oov.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tfe.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lez.jianghu66.top

================================================================================
来源：http://xoa.uphjek.com

K. JSON 与序列化
来源：http://env.vqdsnc.cn

================================================================================
来源：http://lci.nanxuanxn.top

[K01] 对象转 JSON 字符串
来源：http://ktw.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dyk.yongpay.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ggf.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://paq.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://zdq.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uei.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://ixu.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://soq.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ict.gzhubu.top

[K02] JSON 字符串转对象
来源：http://tlc.shangyingyoupin.top

Py:   json.loads(s)
来源：http://mbz.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xxh.iojbl.cn

JS:   JSON.parse(s)
来源：http://bga.shuidangran.top

TS:   JSON.parse(s)
来源：http://obp.jqgufenzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rpi.52xcode.cn

Go:   json.Unmarshal(data, &v)
来源：http://yeg.tarul.cn

Ruby: JSON.parse(s)
来源：http://xsy.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tsw.andypj.xyz

[K03] JSON 美化输出（带缩进）
来源：http://qzr.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bxb.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rya.hcnkem.com

JS:   JSON.stringify(obj, null, 2)
来源：http://drj.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wzs.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://snk.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://txg.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://ijv.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bfj.epnwcf.com

[K04] 读取 JSON 文件
来源：http://fpn.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gex.guannengcc.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bui.zhaomingkeji.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://igd.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wpg.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ywd.bbcook.cn


<!-- 参考信息 -->