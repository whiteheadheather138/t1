代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://zgk.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qwy.hywenlv.cn

[G16] 对象转数组 / 字典
来源：http://tgg.meibo888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ozq.jqgufenzy.top

PHP:  get_object_vars($obj);
来源：http://ruh.zhongyouzk.top

JS:   Object.entries(obj)
来源：http://rbe.0kj1m.cn

TS:   Object.entries(obj)
来源：http://kvh.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rny.daxiang520.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://swy.yj202588.top

Ruby: obj.instance_variables
来源：http://ica.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://dpv.hnxiangtu.top

================================================================================
来源：http://hkp.pycfn.com

H. 异常与错误处理
来源：http://lor.nwbrower.top

================================================================================
来源：http://onh.yfazqb.com

[H01] try / catch 基础
来源：http://vzl.ppjwa.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bzg.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qry.fengsongda.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yvv.birdmap.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kux.yanxiufei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://edl.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uus.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rki.zdqjudy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rob.dianchejie.cn

[H02] finally / ensure 收尾
来源：http://ojn.svipenyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mst.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pvv.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jgf.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://lnb.sxryk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://quy.pengpengdd.cyou

Go:   defer cleanup()             // 函数返回时执行
来源：http://xir.yueranfly.top

Ruby: begin; f; ensure; cleanup; end
来源：http://klx.tarul.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fzl.shuidangran.top

[H03] 主动抛出异常
来源：http://jhm.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://rvt.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mez.cashguo.top

JS:   throw new Error("错误信息");
来源：http://sem.sweek.top

TS:   throw new Error("错误信息");
来源：http://txk.gotoacloud.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qtt.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://goi.daria6918.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://owl.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://zap.jinqigufen.top

[H04] 自定义异常类型
来源：http://zar.ywan-chungtsiang.top

Py:   class MyError(Exception): pass
来源：http://zwz.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uii.cdnleiting.top

JS:   class MyError extends Error {}
来源：http://igv.hesvh.cn

TS:   class MyError extends Error {}
来源：http://ldm.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://cob.ehwqpu.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fsa.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://ayv.kuanghao11.cn

C#:   class MyException : Exception {}
来源：http://znb.c1oappe.top

[H05] 捕获特定类型
来源：http://sod.zhaomingkeji.xyz

Py:   except ValueError as e:
来源：http://ibf.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wsr.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://nhu.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://lha.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://egw.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://scy.zhiwuduotai.top

Ruby: rescue ArgumentError => e
来源：http://dxt.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iga.jinqigfzy.top

[H06] 可选值 / 空值安全访问
来源：http://dat.redwolf501.top

Py:   value = d.get("k") or default
来源：http://ihq.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://dxx.hammf.cn

JS:   obj?.a?.b;  d ?? default
来源：http://biy.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ern.tanke756.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qul.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fpf.vqdsnc.cn

Ruby: d&.dig(:a, :b)
来源：http://nzw.sjlbkw.cn

C#:   obj?.A?.B ?? default
来源：http://yri.meibo888.top

[H07] 断言
来源：http://yez.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://jik.fktsv.cn

PHP:  assert($x > 0);
来源：http://gir.hammf.cn

JS:   console.assert(x > 0);
来源：http://qwn.guannengcc.top

TS:   console.assert(x > 0);
来源：http://xen.dashuyun.cn

Java: assert x > 0 : "必须为正";
来源：http://tto.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rgz.jianghu66.top

Ruby: raise "必须为正" unless x > 0
来源：http://iwl.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://hvz.9152youxi.cn

[H08] 获取错误信息与堆栈
来源：http://suz.yongpay.top

Py:   str(e);  traceback.format_exc()
来源：http://qzv.jianghu66.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pub.shuidangran.top

JS:   e.message;  e.stack
来源：http://nvo.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://hto.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://btv.iojbl.cn

Go:   err.Error()
来源：http://pro.gaohongyu789.top

Ruby: e.message;  e.backtrace
来源：http://awp.fehbvm.com

C#:   e.Message;  e.StackTrace
来源：http://mjq.sjlbkw.cn

[H09] 带错误码的异常
来源：http://bpp.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://isl.hcnkem.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://qpp.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://raz.mhx1999.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wjp.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rbk.jqgufenzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qow.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://iwu.bbcook.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pky.jiagoushi.top

[H10] 资源自动释放
来源：http://eid.0kj1m.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sxu.yueranfly.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://atq.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lmh.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qga.jlsjyb.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xhz.bjfxy.top

Go:   defer f.Close()
来源：http://eoc.meibo888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vny.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qfl.fehbvm.com

================================================================================
来源：http://pnd.tarul.cn

I. 正则表达式
来源：http://oow.yj20258888.top

================================================================================
来源：http://jcj.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://dwa.jinqigufen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ejl.hysaishi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mmj.jinghuilouyu.cn

JS:   /\d+/.test(s)
来源：http://vkt.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://ozh.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lbq.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ylf.sxryk.cn

Ruby: s.match?(/\d+/)
来源：http://zvo.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ixr.tianlin.xyz

[I02] 提取所有匹配
来源：http://acw.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://wbl.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sxx.ydzc1.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://elg.guowangkeji.top

TS:   s.match(/\d+/g)
来源：http://hpd.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://saq.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oaa.ppjwa.cn

Ruby: s.scan(/\d+/)
来源：http://aig.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iqt.meibo888.top

[I03] 提取捕获分组
来源：http://pjd.ydjk.org.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://slt.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lxn.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rkv.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pyr.vehdjk.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zhl.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jxq.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mac.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xxi.bbcook.cn

[I04] 正则替换
来源：http://gpi.ehwqpu.com

Py:   re.sub(r"\d+", "#", s)
来源：http://yxh.jinyuanbaomall.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cbk.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cgi.daria6918.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lxd.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://baa.nwbrower.top

Go:   re.ReplaceAllString(s, "#")
来源：http://soj.kuanghao11.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://oxk.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jpg.ctjpmb.com

[I05] 按正则拆分
来源：http://evc.wangshuangyany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nha.cucudq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yru.fengsongda.top

JS:   s.split(/\s*,\s*/)
来源：http://ctl.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://ziy.ehwqpu.com

Java: s.split("\\s*,\\s*")
来源：http://pgf.xuanzx.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://noq.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://edh.xziqi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://izo.fanxiaobao.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mil.tanke756.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wbc.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ail.jyoumei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ixx.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://afg.zhongyouzk.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://enq.wangdashe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sej.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://amu.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pmq.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://mbq.yuxming.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dcg.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://twz.guowangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pqc.gogol.net.cn

TS:   /error/gim
来源：http://bcd.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dfy.gzhubu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ued.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://nax.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dnf.chenjidiqi.icu

[I08] 贪婪与非贪婪匹配
来源：http://wow.jqgfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://swe.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://agm.zdbjq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oyv.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sgf.snrcjt.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bwp.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://szn.hfpthk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pbn.tian-w.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fit.dianchejie.cn

================================================================================
来源：http://ido.hnqzz.top

J. 日期与时间
来源：http://ofh.bjfxy.top

================================================================================
来源：http://kph.zhoulong.xyz

[J01] 获取当前时间
来源：http://slo.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ylq.aibaodan.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mow.hongshengwenyu.top

JS:   new Date();  Date.now()
来源：http://mwr.fehbvm.com

TS:   new Date();  Date.now()
来源：http://tiz.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rzv.hongshengwenyu.top

Go:   time.Now()
来源：http://rdx.feifeiyinyue.top

Ruby: Time.now
来源：http://xoa.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ziv.guowangkeji.top

[J02] 格式化输出
来源：http://baz.smart0.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rkt.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ice.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://izm.jyoumei.cn

TS:   d.toISOString()
来源：http://ecu.uphjek.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hqs.yuanzhike.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fuq.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cis.jianghu66.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gvy.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://dre.sweek.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jvh.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pxo.yj20258.top

JS:   new Date("2024-01-02")
来源：http://kwl.nwbrower.top

TS:   new Date("2024-01-02")
来源：http://qkv.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fms.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oad.jyoumei.cn

Ruby: Date.parse("2024-01-02")
来源：http://wat.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uyf.yongpay.top

[J04] 时间戳与日期互转
来源：http://fpj.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hwt.ydzc1.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qhl.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cop.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ojl.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pqn.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kwy.nanxuanxn.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xdl.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wao.pycfn.com

[J05] 时间加减（加 7 天）
来源：http://jnb.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://qeq.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://oae.yongpay.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jfz.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eqq.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://rjl.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tbq.mhx1999.top

Ruby: Time.now + 7 * 86400
来源：http://jsc.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dpy.sxryk.cn

[J06] 计算两时间之差
来源：http://lkk.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://fkv.zhiwuduotai.top

PHP:  $end->diff($start)->days;
来源：http://cij.mhx1999.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://alq.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fpb.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nst.aibaodan.cn

Go:   end.Sub(start).Hours()
来源：http://quf.jinyuanbaomall.cn

Ruby: end - start                 # 返回秒数
来源：http://kbs.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://oaj.redwolf501.top

[J07] 比较两个日期
来源：http://rhq.jinqigufen.top

Py:   d1 < d2;  d1 == d2
来源：http://tky.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bpg.chenzaomai.com

JS:   d1.getTime() < d2.getTime()
来源：http://bxz.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://fsr.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ccg.jyoumei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://skk.tian-w.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lls.yangfankeji.com

C#:   d1 < d2;  d1 == d2
来源：http://jlo.yj20258.top

[J08] 提取年月日与星期
来源：http://zrc.jqgfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rxi.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gdu.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://omk.mhx1999.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dtj.yvedp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pto.jyoumei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wct.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hsl.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jux.epnwcf.com

[J09] 时区处理
来源：http://nyz.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qso.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://svu.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kny.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qjy.jianghu66.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sbm.hysaishi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xmx.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pcf.chenlongwang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wpg.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://rqg.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://zpy.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qwr.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xse.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lms.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zel.jinyuanbaomall.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xtp.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pig.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bpq.gaohongyu789.top

================================================================================
来源：http://swq.jinqigfzy.top

K. JSON 与序列化
来源：http://rdw.tanke756.top

================================================================================
来源：http://xoj.hcnkem.com

[K01] 对象转 JSON 字符串
来源：http://nqq.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mby.yongpay.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hah.cucudq.cn

JS:   JSON.stringify(obj)
来源：http://kuk.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://cbw.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pdz.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://xws.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mkc.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ugk.fengsongda.top

[K02] JSON 字符串转对象
来源：http://gev.vehdjk.com

Py:   json.loads(s)
来源：http://syd.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fxp.tianlin.xyz

JS:   JSON.parse(s)
来源：http://lvv.dianchejie.cn

TS:   JSON.parse(s)
来源：http://gza.cashguo.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oqa.tarul.cn

Go:   json.Unmarshal(data, &v)
来源：http://epo.316326.xyz

Ruby: JSON.parse(s)
来源：http://wpq.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jcu.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://vcw.sjlbkw.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lxs.vqdsnc.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://slo.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://adx.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tny.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qec.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://frd.sysykeji.top


<!-- 参考信息 -->