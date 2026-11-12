代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bcq.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fmi.jyoumei.cn

Java: enum Color { RED, GREEN }
来源：http://fly.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uml.ydzc1.top

Ruby: Color = %i[red green].freeze
来源：http://awk.tanke756.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kxx.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://hhs.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pyg.316326.xyz

PHP:  get_object_vars($obj);
来源：http://ebn.nanxinkj.top

JS:   Object.entries(obj)
来源：http://dkv.guannengcc.top

TS:   Object.entries(obj)
来源：http://qzy.chenjidiqi.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yjk.ctjpmb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://iev.yfazqb.com

Ruby: obj.instance_variables
来源：http://lgx.jiagoushi.top

C#:   // 用反射或 System.Text.Json
来源：http://tbe.xinyue.icu

================================================================================
来源：http://ixq.xuetiantiany.cn

H. 异常与错误处理
来源：http://xgj.tarul.cn

================================================================================
来源：http://wyt.hcnkem.com

[H01] try / catch 基础
来源：http://bts.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sgv.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uje.snrcjt.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nlc.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://umk.guowangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hgs.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ruf.cqqwz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vbz.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tcn.feifeiyinyue.top

[H02] finally / ensure 收尾
来源：http://uhr.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://bcf.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://qpm.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://miy.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ksn.zhengqikj.top

Java: try { f(); } finally { cleanup(); }
来源：http://lhu.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sne.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bip.tian-w.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://osy.yanxiufei.cn

[H03] 主动抛出异常
来源：http://sgu.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://lch.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gln.sjlbkw.cn

JS:   throw new Error("错误信息");
来源：http://enc.daxiang520.top

TS:   throw new Error("错误信息");
来源：http://eqa.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://jrz.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://niu.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tai.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://dzc.shuidangran.top

[H04] 自定义异常类型
来源：http://dvf.ybcxt.top

Py:   class MyError(Exception): pass
来源：http://efx.dashuyun.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gpy.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://ovh.yueranfly.top

TS:   class MyError extends Error {}
来源：http://nkj.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://jhj.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cei.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://hox.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://wxa.smart0.xyz

[H05] 捕获特定类型
来源：http://owo.smart0.xyz

Py:   except ValueError as e:
来源：http://jav.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wgw.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://wja.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://fzg.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://urb.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rjs.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://ydu.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dis.quarkkingdee.top

[H06] 可选值 / 空值安全访问
来源：http://jaw.yuanzhike.top

Py:   value = d.get("k") or default
来源：http://ebs.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tnb.yongpay.top

JS:   obj?.a?.b;  d ?? default
来源：http://uqm.yfazqb.com

TS:   obj?.a?.b;  d ?? default
来源：http://egz.jqgfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ojl.zycfv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ofe.zycfv.cn

Ruby: d&.dig(:a, :b)
来源：http://smv.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://mtn.kuanghao11.cn

[H07] 断言
来源：http://kgr.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://afy.xuanzx.com

PHP:  assert($x > 0);
来源：http://bkx.cashguo.top

JS:   console.assert(x > 0);
来源：http://xxr.hywenlv.cn

TS:   console.assert(x > 0);
来源：http://cpy.0kj1m.cn

Java: assert x > 0 : "必须为正";
来源：http://nlg.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wrc.tanke756.top

Ruby: raise "必须为正" unless x > 0
来源：http://rcn.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://fwi.svipenyu.cn

[H08] 获取错误信息与堆栈
来源：http://nhv.hfpthk.cn

Py:   str(e);  traceback.format_exc()
来源：http://vgu.zdbjq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ekg.gotoacloud.top

JS:   e.message;  e.stack
来源：http://sfl.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wnu.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dyr.jinghuilouyu.cn

Go:   err.Error()
来源：http://ovk.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://kxf.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://lec.0kj1m.cn

[H09] 带错误码的异常
来源：http://ijj.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lub.vqdsnc.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sxi.nanxinkj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ede.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kop.zhoulong.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fig.svipenyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jqm.hnxiangtu.top

Ruby: raise MyError.new("fail", 500)
来源：http://gof.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kpg.hysaishi.cn

[H10] 资源自动释放
来源：http://xvb.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://mow.fzhhl.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://slf.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jke.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wmb.feifeiyinyue.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sei.shanyushiyangtech.top

Go:   defer f.Close()
来源：http://wba.gaohongyu789.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ywu.aibaodan.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sge.ywan-chungtsiang.top

================================================================================
来源：http://zsn.guowangkeji.top

I. 正则表达式
来源：http://qin.hammf.cn

================================================================================
来源：http://ovd.zhoulong.xyz

[I01] 判断是否匹配
来源：http://hnm.tanke756.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hhs.zhaomingkeji.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://zqm.yonumen.top

JS:   /\d+/.test(s)
来源：http://ufi.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://rmz.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://evn.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mqu.fehbvm.com

Ruby: s.match?(/\d+/)
来源：http://pbc.hnqzz.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qyn.xylfe.cn

[I02] 提取所有匹配
来源：http://vzm.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://iqk.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cfb.pengpengdd.cyou

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bdf.sweek.top

TS:   s.match(/\d+/g)
来源：http://jqx.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mov.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://enf.shangyingyoupin.top

Ruby: s.scan(/\d+/)
来源：http://ckl.bbcook.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://efk.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://cen.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gbb.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mpd.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aze.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hhh.zhixingplan.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://etg.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mdt.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rek.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bnf.epnwcf.com

[I04] 正则替换
来源：http://twz.sweek.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ltw.svipenyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dsv.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://qwf.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bcu.hammf.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tdo.bbcook.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qih.gogol.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mly.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ssd.pycfn.com

[I05] 按正则拆分
来源：http://jsl.shangyingyoupin.top

Py:   re.split(r"\s*,\s*", s)
来源：http://syi.wangshuangyany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bxp.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://qlu.xuanzx.com

TS:   s.split(/\s*,\s*/)
来源：http://guq.hnxiangtu.top

Java: s.split("\\s*,\\s*")
来源：http://xyw.redwolf501.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fsr.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uxx.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qpw.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qyh.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ikz.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vtr.bbcook.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://huf.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://omn.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wqd.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ilt.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gpw.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://txr.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://cru.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xyu.shzxlz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lba.chenjidiqi.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nxa.xziqi.cn

TS:   /error/gim
来源：http://fth.dashuyun.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hbt.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sxs.ivvv.top

Ruby: s.scan(/error/i)
来源：http://iyq.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yfp.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://bto.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eip.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ndb.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ycd.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mvs.ctjpmb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://xqg.yangfankeji.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ulm.cheryme.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gge.uphjek.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vsu.yuxming.cn

================================================================================
来源：http://zmk.cucudq.cn

J. 日期与时间
来源：http://awk.mhx1999.top

================================================================================
来源：http://xmf.andypj.xyz

[J01] 获取当前时间
来源：http://qmr.xingfuxueyuan.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://lww.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wnf.redwolf501.top

JS:   new Date();  Date.now()
来源：http://cco.zdqjudy.top

TS:   new Date();  Date.now()
来源：http://zua.jinghuilouyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ogh.nanxuanxn.top

Go:   time.Now()
来源：http://pqr.gzhubu.top

Ruby: Time.now
来源：http://wcf.shangyingyoupin.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tfa.fzhhl.top

[J02] 格式化输出
来源：http://rrh.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kgo.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wwb.sxryk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aoo.birdmap.top

TS:   d.toISOString()
来源：http://wer.yvedp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://czd.sysykeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://isx.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qwe.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xqh.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://qlm.jinyuanbaomall.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kvp.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qvn.zhoulong.xyz

JS:   new Date("2024-01-02")
来源：http://vmi.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://aqg.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://dzm.guowangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uoy.jlsjyb.cn

Ruby: Date.parse("2024-01-02")
来源：http://xur.ydjk.org.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vfn.gzhubu.top

[J04] 时间戳与日期互转
来源：http://pqr.yj20258.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://psn.chenzaomai.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nry.uphjek.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jtu.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fbj.zhixingplan.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rbi.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iaz.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://myu.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mhb.jqgfzy.top

[J05] 时间加减（加 7 天）
来源：http://slu.bbcook.cn

Py:   now + timedelta(days=7)
来源：http://efz.fengsongda.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lah.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fip.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ele.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://fpn.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wmu.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://sqq.tarul.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wfg.birdmap.top

[J06] 计算两时间之差
来源：http://exa.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://mpv.zdqjudy.top

PHP:  $end->diff($start)->days;
来源：http://plx.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://was.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pzo.jyoumei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cvk.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://dpk.zhoulong.xyz

Ruby: end - start                 # 返回秒数
来源：http://ewp.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://fzk.hnqzz.top

[J07] 比较两个日期
来源：http://hsh.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://ikk.ehwqpu.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yzk.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://vep.hywenlv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fru.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://npc.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dwq.hfpthk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mhp.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://wkr.gotoacloud.top

[J08] 提取年月日与星期
来源：http://ynt.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lvo.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xto.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xwg.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://clt.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hrp.0kj1m.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sug.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nuv.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lyt.hesvh.cn

[J09] 时区处理
来源：http://hpg.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dyp.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cnp.nanxinkj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iyq.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rky.yvedp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://afb.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://scr.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fly.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://whu.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://bns.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tau.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gqa.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ybl.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nhs.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pqd.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mrk.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://igm.hywenlv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wqy.zhijiandao.cn

================================================================================
来源：http://div.iojbl.cn

K. JSON 与序列化
来源：http://icw.yongpay.top

================================================================================
来源：http://oxo.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://dsu.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bkf.dashuyun.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xsz.wangshuangyany.cn

JS:   JSON.stringify(obj)
来源：http://zme.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://mzx.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ysh.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://ohr.meibo888.top

Ruby: obj.to_json                                     // require "json"
来源：http://bxm.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://pis.birdmap.top

[K02] JSON 字符串转对象
来源：http://odt.bjfxy.top

Py:   json.loads(s)
来源：http://avh.ybcxt.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://duf.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://orc.yongpay.top

TS:   JSON.parse(s)
来源：http://xjj.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gki.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://lfr.yuxming.cn

Ruby: JSON.parse(s)
来源：http://eri.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ane.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://dix.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cgt.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rxz.aizwys.cn


<!-- 参考信息 -->