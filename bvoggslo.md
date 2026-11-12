代发 wailian999

C#:   record User(string Name, int Age);
来源：http://bne.jinqigufen.top

[G15] 枚举
来源：http://bla.ywan-chungtsiang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tke.tanke756.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zyf.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://afy.nanxuanxn.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xpk.yj20258.top

Java: enum Color { RED, GREEN }
来源：http://tqi.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zxb.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://gev.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gat.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://ssa.havefunace.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wog.yj20258.top

PHP:  get_object_vars($obj);
来源：http://qzg.shzxlz.cn

JS:   Object.entries(obj)
来源：http://ymp.snrcjt.cn

TS:   Object.entries(obj)
来源：http://ykx.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mxy.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nya.xziqi.cn

Ruby: obj.instance_variables
来源：http://box.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://jni.dianchejie.cn

================================================================================
来源：http://pqi.nanxuanxn.top

H. 异常与错误处理
来源：http://qgz.andypj.xyz

================================================================================
来源：http://ajf.hesvh.cn

[H01] try / catch 基础
来源：http://nha.hcnkem.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lll.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vrf.xziqi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dvu.birdmap.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yoa.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hjw.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yxs.xingfuxueyuan.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ymk.c1oappe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ntl.daria6918.cn

[H02] finally / ensure 收尾
来源：http://xlg.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://qve.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ndf.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xxt.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://jmj.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pzx.fktsv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hoi.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ldl.shanyushiyangtech.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gmm.snrcjt.cn

[H03] 主动抛出异常
来源：http://nlu.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://idl.sjlbkw.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mzq.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://vqp.yueranfly.top

TS:   throw new Error("错误信息");
来源：http://orq.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jxi.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xue.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pqj.jqgfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://rja.kuanghao11.cn

[H04] 自定义异常类型
来源：http://fss.hfpthk.cn

Py:   class MyError(Exception): pass
来源：http://qjr.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://iri.yj20258.top

JS:   class MyError extends Error {}
来源：http://bml.havefunace.top

TS:   class MyError extends Error {}
来源：http://xyl.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://bag.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tlg.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://yje.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://qsk.52xcode.cn

[H05] 捕获特定类型
来源：http://qnt.shangyingyoupin.top

Py:   except ValueError as e:
来源：http://ayv.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cuu.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://zas.hfpthk.cn

TS:   if (e instanceof TypeError) {}
来源：http://wiw.hongshengwenyu.top

Java: catch (IOException | SQLException e) {}
来源：http://wuc.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ynh.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://moh.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sum.jinqigfzy.top

[H06] 可选值 / 空值安全访问
来源：http://djq.ydjk.org.cn

Py:   value = d.get("k") or default
来源：http://irz.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://rlk.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jok.chenlongwang.top

TS:   obj?.a?.b;  d ?? default
来源：http://hjd.hcnkem.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://guy.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zfa.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://bfm.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://scw.wangshuangyany.cn

[H07] 断言
来源：http://idj.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://ipd.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://btb.haohaochexian.top

JS:   console.assert(x > 0);
来源：http://avq.jiagoushi.top

TS:   console.assert(x > 0);
来源：http://oko.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://tfy.fehbvm.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pqu.tanke756.top

Ruby: raise "必须为正" unless x > 0
来源：http://jaz.52xcode.cn

C#:   Debug.Assert(x > 0);
来源：http://ale.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://bua.sysykeji.top

Py:   str(e);  traceback.format_exc()
来源：http://sdx.jiagoushi.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rom.zdbjq.cn

JS:   e.message;  e.stack
来源：http://fij.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://hti.zhiwuduotai.top

Java: e.getMessage();  e.printStackTrace()
来源：http://slx.yueranfly.top

Go:   err.Error()
来源：http://iqr.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://dwn.hysaishi.cn

C#:   e.Message;  e.StackTrace
来源：http://tig.jinqigfzy.top

[H09] 带错误码的异常
来源：http://czb.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kgf.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://noz.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ynb.vqdsnc.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tlv.yj20258.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qcv.hfpthk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://alt.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hhv.pengpengdd.cyou

C#:   // 自定义异常类中加 Code 属性
来源：http://fcj.chenjidiqi.icu

[H10] 资源自动释放
来源：http://qgo.nwbrower.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wiq.zhaomingkeji.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vsl.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://emv.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cvn.uphjek.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yxf.zdbjq.cn

Go:   defer f.Close()
来源：http://vac.xinyue.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ysj.jinyuanbaomall.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fww.dashuyun.cn

================================================================================
来源：http://jts.hnqzz.top

I. 正则表达式
来源：http://zcg.birdmap.top

================================================================================
来源：http://hwr.vehdjk.com

[I01] 判断是否匹配
来源：http://wmm.fktsv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wdc.cheryme.top

PHP:  preg_match('/\d+/', $s);
来源：http://jqg.daxiang520.top

JS:   /\d+/.test(s)
来源：http://ajs.sjlbkw.cn

TS:   /\d+/.test(s)
来源：http://gjt.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ggs.guannengcc.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xin.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://yyl.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rht.9152youxi.cn

[I02] 提取所有匹配
来源：http://pou.cheryme.top

Py:   re.findall(r"\d+", s)
来源：http://zto.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gik.guowangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eis.quarkkingdee.top

TS:   s.match(/\d+/g)
来源：http://fks.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rdw.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vtz.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://ehl.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vxx.nwbrower.top

[I03] 提取捕获分组
来源：http://rjp.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ftv.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fhf.yj20258.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://drr.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://flo.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://div.zhoulong.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mid.chenjidiqi.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://orq.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lwp.shanyushiyangkeji.top

[I04] 正则替换
来源：http://dfu.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zts.zhoulong.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aut.yonumen.top

JS:   s.replace(/\d+/g, "#")
来源：http://ysd.zycfv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vwu.hnqzz.top

Java: s.replaceAll("\\d+", "#")
来源：http://zci.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://okh.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://iul.dianchejie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kqv.haohaochexian.top

[I05] 按正则拆分
来源：http://byg.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kuy.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zdc.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://wxz.zhiwuduotai.top

TS:   s.split(/\s*,\s*/)
来源：http://vip.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://pbv.hcnkem.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wzj.zhijiandao.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ojy.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bii.chenlongwang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cft.hnxiangtu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ibc.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qbw.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ndk.vehdjk.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://msa.feifeiyinyue.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://def.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vre.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://inp.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cgf.cqqwz.cn

[I07] 忽略大小写与多行模式
来源：http://vig.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pup.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xmb.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ozj.shzxlz.cn

TS:   /error/gim
来源：http://ghe.shanyushiyangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bmb.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rrq.ivvv.top

Ruby: s.scan(/error/i)
来源：http://uqv.bbcook.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ixv.shuidangran.top

[I08] 贪婪与非贪婪匹配
来源：http://fky.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://akh.mhx1999.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pru.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vnr.smart0.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bak.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fxd.tanke756.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kzt.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gss.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://soq.nanxinkj.top

================================================================================
来源：http://esh.uphjek.com

J. 日期与时间
来源：http://vcr.smart0.xyz

================================================================================
来源：http://znr.ydzc1.top

[J01] 获取当前时间
来源：http://bzi.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aly.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uyx.cqqwz.cn

JS:   new Date();  Date.now()
来源：http://awg.zhengqikj.top

TS:   new Date();  Date.now()
来源：http://ogh.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://zuv.yfazqb.com

Go:   time.Now()
来源：http://nhf.zhijiandao.cn

Ruby: Time.now
来源：http://jjn.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kmf.ydjk.org.cn

[J02] 格式化输出
来源：http://kvp.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bfe.smart0.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rds.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fxo.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://adj.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jtl.52xcode.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fxc.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nzt.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://abi.sjlbkw.cn

[J03] 字符串解析为日期
来源：http://tek.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lwu.shangyingyoupin.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ksp.ydzc1.top

JS:   new Date("2024-01-02")
来源：http://hsa.fengsongda.top

TS:   new Date("2024-01-02")
来源：http://pcy.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://zoo.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wfm.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://dwq.yj202588.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ssi.fktsv.cn

[J04] 时间戳与日期互转
来源：http://xmk.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fet.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://izb.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bwf.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://brz.52xcode.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://orb.chenjidiqi.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fyn.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cit.gotoacloud.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://two.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://nca.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://ono.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ecf.xziqi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://awn.zdbjq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dkp.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://ece.yvedp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ims.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://teg.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bvy.hammf.cn

[J06] 计算两时间之差
来源：http://pgk.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://fac.zhaomingkeji.xyz

PHP:  $end->diff($start)->days;
来源：http://clc.feifeiyinyue.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kjr.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://maa.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://pyz.nanxinkj.top

Go:   end.Sub(start).Hours()
来源：http://ktw.tianlin.xyz

Ruby: end - start                 # 返回秒数
来源：http://glm.ppjwa.cn

C#:   (end - start).TotalSeconds
来源：http://ujs.shuidangran.top

[J07] 比较两个日期
来源：http://kqo.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://wxe.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vyw.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://vfo.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://jvx.gaohongyu789.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kdn.jiagoushi.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zay.bjfxy.top

Ruby: d1 < d2;  d1 == d2
来源：http://nod.mhx1999.top

C#:   d1 < d2;  d1 == d2
来源：http://vym.nanxuanxn.top

[J08] 提取年月日与星期
来源：http://iwl.tanke756.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wnz.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://beh.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ywb.xziqi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mwi.ydzc1.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cnl.ctjpmb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ric.sufxvd.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nqn.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mmj.gotoacloud.top

[J09] 时区处理
来源：http://bnf.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qid.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zuj.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lrn.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uqd.svipenyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ilm.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ney.haohaochexian.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sqj.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bry.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://bhl.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xas.zhijiandao.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ggg.iojbl.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mdu.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wvj.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nqu.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pww.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://brf.fzhhl.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hdv.havefunace.top

================================================================================
来源：http://rix.jyoumei.cn

K. JSON 与序列化
来源：http://the.0kj1m.cn

================================================================================
来源：http://ogk.hongshengwenyu.top

[K01] 对象转 JSON 字符串
来源：http://zfa.cdnleiting.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pzt.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pbe.andypj.xyz

JS:   JSON.stringify(obj)
来源：http://rym.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://yez.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bfd.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://vrf.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://qen.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gat.nwbrower.top

[K02] JSON 字符串转对象
来源：http://vdr.zycfv.cn

Py:   json.loads(s)
来源：http://ueu.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aeb.zdqjudy.top

JS:   JSON.parse(s)
来源：http://oxw.zhiwuduotai.top

TS:   JSON.parse(s)
来源：http://mmy.quarkkingdee.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zyp.gogol.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://qht.fengsongda.top

Ruby: JSON.parse(s)
来源：http://mvy.cheryme.top


<!-- 参考信息 -->