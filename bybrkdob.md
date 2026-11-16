代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://yoh.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://bws.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://goz.jlsjyb.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hfe.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://wtn.yangfankeji.com

[G15] 枚举
来源：http://vxa.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://okc.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://vgf.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eyz.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hky.ivvv.top

Java: enum Color { RED, GREEN }
来源：http://klh.ywan-chungtsiang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://azf.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://koe.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://apy.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://ctq.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zha.ybcxt.top

PHP:  get_object_vars($obj);
来源：http://izq.ybcxt.top

JS:   Object.entries(obj)
来源：http://ycx.hcnkem.com

TS:   Object.entries(obj)
来源：http://hzf.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gnn.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vza.zdbjq.cn

Ruby: obj.instance_variables
来源：http://dsa.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://ahx.epnwcf.com

================================================================================
来源：http://irf.yueranfly.top

H. 异常与错误处理
来源：http://jgh.dianchejie.cn

================================================================================
来源：http://yep.smart0.xyz

[H01] try / catch 基础
来源：http://khk.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ksj.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eyj.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qpa.jyoumei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tia.chenlongwang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vut.sxryk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wrb.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gkl.xinyue.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wyp.chenjidiqi.icu

[H02] finally / ensure 收尾
来源：http://yta.cheryme.top

Py:   try: f()⏎finally: cleanup()
来源：http://vvb.nanxuanxn.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bqo.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://muc.tanke756.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qmk.ywan-chungtsiang.top

Java: try { f(); } finally { cleanup(); }
来源：http://con.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ugu.jinyuanbaomall.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://goc.cheryme.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xzp.guowangkeji.top

[H03] 主动抛出异常
来源：http://kyp.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://xov.hfpthk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ipa.daxiang520.top

JS:   throw new Error("错误信息");
来源：http://rpc.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://xnr.52xcode.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://byy.daria6918.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://frg.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://umi.ehwqpu.com

C#:   throw new ArgumentException("错误信息");
来源：http://srl.gogol.net.cn

[H04] 自定义异常类型
来源：http://vkd.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://yfo.snrcjt.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gci.bjfxy.top

JS:   class MyError extends Error {}
来源：http://mpy.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://ink.316326.xyz

Java: class MyException extends RuntimeException {}
来源：http://vrs.tarul.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ndh.cashguo.top

Ruby: class MyError < StandardError; end
来源：http://cbp.chenlongwang.top

C#:   class MyException : Exception {}
来源：http://lug.316326.xyz

[H05] 捕获特定类型
来源：http://blu.chenlongwang.top

Py:   except ValueError as e:
来源：http://zez.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wrj.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://bun.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://tyz.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://did.fktsv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lwz.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://dqq.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ykx.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://sdr.guowangkeji.top

Py:   value = d.get("k") or default
来源：http://hee.hcnkem.com

PHP:  $v = $d["k"] ?? null;
来源：http://rml.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://kmn.hammf.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ufs.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://egg.ppjwa.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hov.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://lrn.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://ond.hywenlv.cn

[H07] 断言
来源：http://czd.svipenyu.cn

Py:   assert x > 0, "必须为正"
来源：http://mht.vqdsnc.cn

PHP:  assert($x > 0);
来源：http://erg.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://vfp.hnxiangtu.top

TS:   console.assert(x > 0);
来源：http://rel.dianchejie.cn

Java: assert x > 0 : "必须为正";
来源：http://roy.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fxw.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://okz.wangdashe.top

C#:   Debug.Assert(x > 0);
来源：http://ejx.yuxming.cn

[H08] 获取错误信息与堆栈
来源：http://buc.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://jls.svipenyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wse.xuanzx.com

JS:   e.message;  e.stack
来源：http://ltk.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fiz.hesvh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mue.uphjek.com

Go:   err.Error()
来源：http://paw.zhixingplan.top

Ruby: e.message;  e.backtrace
来源：http://ncs.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://wzt.zhengqikj.top

[H09] 带错误码的异常
来源：http://mja.cashguo.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mwm.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://nbx.gogol.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://szn.yvedp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bhf.nanxuanxn.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cgb.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sdx.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://paw.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mpe.zycfv.cn

[H10] 资源自动释放
来源：http://vku.tian-w.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jec.guannengcc.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vhe.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ksc.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gvs.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qrm.sufxvd.cn

Go:   defer f.Close()
来源：http://ffs.fanxiaobao.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pdz.pycfn.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ebi.zhongyouzk.top

================================================================================
来源：http://wak.hfpthk.cn

I. 正则表达式
来源：http://rnw.jqgfzy.top

================================================================================
来源：http://prl.xziqi.cn

[I01] 判断是否匹配
来源：http://ovc.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://otm.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jku.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://qph.xuanzx.com

TS:   /\d+/.test(s)
来源：http://bxl.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uyg.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://krb.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://cel.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://klm.sufxvd.cn

[I02] 提取所有匹配
来源：http://dyo.jinghuilouyu.cn

Py:   re.findall(r"\d+", s)
来源：http://acu.jqgfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ivy.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cyj.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://jsp.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zap.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ehz.shangyingyoupin.top

Ruby: s.scan(/\d+/)
来源：http://jab.hcnkem.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gud.cucudq.cn

[I03] 提取捕获分组
来源：http://oje.nwbrower.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mrs.pycfn.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dnt.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zqs.meibo888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oyx.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xbx.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kdz.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zka.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wse.snrcjt.cn

[I04] 正则替换
来源：http://dnb.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pji.zhongyouzk.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tnl.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://azx.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://gny.birdmap.top

Java: s.replaceAll("\\d+", "#")
来源：http://uwo.ydjk.org.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mqu.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ptm.gotoacloud.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mrb.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://aak.gaohongyu789.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cax.chenzaomai.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://riq.yangfankeji.com

JS:   s.split(/\s*,\s*/)
来源：http://pya.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://ahg.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://wzn.havefunace.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fjs.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://bkt.pengpengdd.cyou

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vzw.birdmap.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ryi.shzxlz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qxl.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oog.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zii.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mlt.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fqq.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://huu.epnwcf.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oqg.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uqe.pengpengdd.cyou

[I07] 忽略大小写与多行模式
来源：http://xwc.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xjp.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bmw.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iuj.zhaomingkeji.xyz

TS:   /error/gim
来源：http://ntn.sxryk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iym.chenlongwang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gbe.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://ybj.birdmap.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tsg.hammf.cn

[I08] 贪婪与非贪婪匹配
来源：http://lyn.jqgfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://imz.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://edu.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ncu.tian-w.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://obh.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ngj.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fey.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mbj.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rdx.tianlin.xyz

================================================================================
来源：http://abp.epnwcf.com

J. 日期与时间
来源：http://ebn.kuanghao11.cn

================================================================================
来源：http://voi.xylfe.cn

[J01] 获取当前时间
来源：http://dmq.quarkkingdee.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xqr.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ape.yangfankeji.com

JS:   new Date();  Date.now()
来源：http://ypk.zycfv.cn

TS:   new Date();  Date.now()
来源：http://zrx.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oid.vqdsnc.cn

Go:   time.Now()
来源：http://ebn.yj20258888.top

Ruby: Time.now
来源：http://hla.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://psp.zdqjudy.top

[J02] 格式化输出
来源：http://hja.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lng.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dbu.tianlin.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hhe.jinghuilouyu.cn

TS:   d.toISOString()
来源：http://wue.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lhp.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bay.wangdashe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ilh.yvedp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lpq.ybcxt.top

[J03] 字符串解析为日期
来源：http://nnu.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jxh.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://exm.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://kau.tarul.cn

TS:   new Date("2024-01-02")
来源：http://seb.xingfuxueyuan.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://sbb.zhaomingkeji.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://for.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://ncl.zhaomingkeji.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ixo.sjlbkw.cn

[J04] 时间戳与日期互转
来源：http://mxe.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zhl.yonumen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lpw.hcnkem.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mpa.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://unx.hywenlv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cay.cheryme.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gog.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vos.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hhr.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://xqs.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://wut.hywenlv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vbm.feifeiyinyue.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yqo.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wlb.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://bwq.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qhd.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://nwr.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://apx.vqdsnc.cn

[J06] 计算两时间之差
来源：http://yti.kuanghao11.cn

Py:   (end - start).total_seconds()
来源：http://pol.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://ntt.hongshengwenyu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ccc.xingfuxueyuan.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xqu.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://quh.sjlbkw.cn

Go:   end.Sub(start).Hours()
来源：http://wyl.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://zzf.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://rbn.zhongyouzk.top

[J07] 比较两个日期
来源：http://yaf.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ezb.xziqi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yna.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://igu.xuetiantiany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://slw.uphjek.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dij.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aea.hywenlv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://obq.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://ngx.quarkkingdee.top

[J08] 提取年月日与星期
来源：http://tpb.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bzl.guowangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xsi.jqgufenzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fzg.wangdashe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://peh.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jwu.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qwx.zhengqikj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://msa.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ahl.haohaochexian.top

[J09] 时区处理
来源：http://kxy.chenjidiqi.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yhy.jlsjyb.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qkb.zhijiandao.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ogy.gaohongyu789.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lxy.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cfp.yuxming.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zwe.jiagoushi.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dae.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ezc.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://jyy.gogol.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hqw.52xcode.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kfq.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nlz.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rim.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qyj.cashguo.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zkz.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://izn.pengpengdd.cyou

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xfw.jyoumei.cn

================================================================================
来源：http://jzr.redwolf501.top

K. JSON 与序列化
来源：http://qup.hysaishi.cn

================================================================================
来源：http://jzr.ivvv.top

[K01] 对象转 JSON 字符串
来源：http://voa.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xtx.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ojp.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://ims.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://trb.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wbs.tarul.cn

Go:   json.Marshal(obj)
来源：http://nlv.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://hth.meibo888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vxy.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://lwl.cqqwz.cn

Py:   json.loads(s)
来源：http://bzt.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pmv.tian-w.cn

JS:   JSON.parse(s)
来源：http://prc.epnwcf.com


<!-- 参考信息 -->