代发 wailian999

C#:   record User(string Name, int Age);
来源：http://vtr.zycfv.cn

[G15] 枚举
来源：http://adc.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ohy.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fnc.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wuc.ctjpmb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ife.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://jnn.fktsv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xqm.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://qzh.quarkkingdee.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bkw.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://wuh.svipenyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cgw.ybcxt.top

PHP:  get_object_vars($obj);
来源：http://zer.gzhubu.top

JS:   Object.entries(obj)
来源：http://phe.havefunace.top

TS:   Object.entries(obj)
来源：http://tuj.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ljv.daxiang520.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hjm.smart0.xyz

Ruby: obj.instance_variables
来源：http://kge.zhixingplan.top

C#:   // 用反射或 System.Text.Json
来源：http://wfr.uphjek.com

================================================================================
来源：http://tku.wangshuangyany.cn

H. 异常与错误处理
来源：http://nzg.haohaochexian.top

================================================================================
来源：http://pmq.yfazqb.com

[H01] try / catch 基础
来源：http://kii.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pic.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://opc.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rjh.tanke756.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fxr.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ori.jlsjyb.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dwi.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jjl.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rle.hywenlv.cn

[H02] finally / ensure 收尾
来源：http://aje.xylfe.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ozp.chenlongwang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cpr.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qxr.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://row.hnqzz.top

Java: try { f(); } finally { cleanup(); }
来源：http://lya.sxryk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nyl.fanxiaobao.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://jed.sjlbkw.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bzr.pycfn.com

[H03] 主动抛出异常
来源：http://may.dashuyun.cn

Py:   raise ValueError("错误信息")
来源：http://mwj.feifeiyinyue.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sfo.cashguo.top

JS:   throw new Error("错误信息");
来源：http://jdl.wangdashe.top

TS:   throw new Error("错误信息");
来源：http://fex.xuanzx.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://nbe.jqgfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ioy.cdnleiting.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lci.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://mmx.daxiang520.top

[H04] 自定义异常类型
来源：http://swt.yfazqb.com

Py:   class MyError(Exception): pass
来源：http://lsl.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://hck.yanxiufei.cn

JS:   class MyError extends Error {}
来源：http://nwh.sjlbkw.cn

TS:   class MyError extends Error {}
来源：http://ukl.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://yxf.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rfk.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://qji.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://jkq.cucudq.cn

[H05] 捕获特定类型
来源：http://xxt.svipenyu.cn

Py:   except ValueError as e:
来源：http://fdp.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://byu.ydzc1.top

JS:   if (e instanceof TypeError) {}
来源：http://sgj.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://qki.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://afs.sufxvd.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gyv.fanxiaobao.xyz

Ruby: rescue ArgumentError => e
来源：http://rpi.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://goy.mhx1999.top

[H06] 可选值 / 空值安全访问
来源：http://abm.shangyingyoupin.top

Py:   value = d.get("k") or default
来源：http://xur.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://ckl.jinqigfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://ryd.vehdjk.com

TS:   obj?.a?.b;  d ?? default
来源：http://pyd.hnqzz.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vdu.hammf.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ixi.zhaomingkeji.xyz

Ruby: d&.dig(:a, :b)
来源：http://xxm.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://kbj.yvedp.cn

[H07] 断言
来源：http://ngh.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://lzd.birdmap.top

PHP:  assert($x > 0);
来源：http://kne.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://lnn.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://cwk.yueranfly.top

Java: assert x > 0 : "必须为正";
来源：http://whh.zdqjudy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pzx.cqqwz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bby.xingfuxueyuan.xyz

C#:   Debug.Assert(x > 0);
来源：http://jhk.wangdashe.top

[H08] 获取错误信息与堆栈
来源：http://ylg.sweek.top

Py:   str(e);  traceback.format_exc()
来源：http://ddd.jlsjyb.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://szp.tian-w.cn

JS:   e.message;  e.stack
来源：http://jjc.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bxd.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ozp.ctjpmb.com

Go:   err.Error()
来源：http://xjx.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://pfx.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://plp.zdbjq.cn

[H09] 带错误码的异常
来源：http://zbj.redwolf501.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lmj.shangyingyoupin.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mwm.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cvo.zhengqikj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gem.xingfuxueyuan.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fsb.aizwys.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gqj.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rqf.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bwm.zhijiandao.cn

[H10] 资源自动释放
来源：http://rhx.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wsn.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zrx.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zzn.xuetiantiany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fpb.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aqq.52xcode.cn

Go:   defer f.Close()
来源：http://scz.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://trl.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bhn.yonumen.top

================================================================================
来源：http://ppt.tian-w.cn

I. 正则表达式
来源：http://asz.sweek.top

================================================================================
来源：http://xna.sysykeji.top

[I01] 判断是否匹配
来源：http://vzp.epnwcf.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://opp.wangshuangyany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://orb.hammf.cn

JS:   /\d+/.test(s)
来源：http://rbh.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://ckt.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rwz.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dkc.cucudq.cn

Ruby: s.match?(/\d+/)
来源：http://gdg.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gjo.guowangkeji.top

[I02] 提取所有匹配
来源：http://rzg.daxiang520.top

Py:   re.findall(r"\d+", s)
来源：http://lqn.vqdsnc.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://anj.jiagoushi.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ffy.ydzc1.top

TS:   s.match(/\d+/g)
来源：http://jey.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zcy.xziqi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xqm.jinqigufen.top

Ruby: s.scan(/\d+/)
来源：http://vpu.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fwd.xuanzx.com

[I03] 提取捕获分组
来源：http://yey.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kzp.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tpj.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://agx.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kde.fzhhl.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hvk.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nvc.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mdu.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cmp.jqgufenzy.top

[I04] 正则替换
来源：http://ivo.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fot.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wfz.xinyue.icu

JS:   s.replace(/\d+/g, "#")
来源：http://tbo.0kj1m.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pea.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://adz.aizwys.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oxa.yfazqb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://erk.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://taw.yongpay.top

[I05] 按正则拆分
来源：http://hfq.jianghu66.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mar.chenlongwang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vat.epnwcf.com

JS:   s.split(/\s*,\s*/)
来源：http://jua.havefunace.top

TS:   s.split(/\s*,\s*/)
来源：http://qvw.hnqzz.top

Java: s.split("\\s*,\\s*")
来源：http://tfu.fktsv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kqg.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nfr.pycfn.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pew.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zji.0kj1m.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mdq.fzhhl.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qvy.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xzk.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jcl.yongpay.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lnw.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ldg.iojbl.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vud.chenlongwang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nvc.jinyuanbaomall.cn

[I07] 忽略大小写与多行模式
来源：http://qmb.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oiq.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zkm.havefunace.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dwp.nanxuanxn.top

TS:   /error/gim
来源：http://xch.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wif.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://osg.cashguo.top

Ruby: s.scan(/error/i)
来源：http://dwe.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://utb.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://bwx.nanxuanxn.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iib.sysykeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nip.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://adl.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://czj.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://otp.sweek.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uua.cheryme.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://str.wangdashe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vvj.hnqzz.top

================================================================================
来源：http://yqr.316326.xyz

J. 日期与时间
来源：http://bay.jqgufenzy.top

================================================================================
来源：http://ebn.jinqigfzy.top

[J01] 获取当前时间
来源：http://mby.hfpthk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mwe.pengpengdd.cyou

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vlz.xziqi.cn

JS:   new Date();  Date.now()
来源：http://cal.guannengcc.top

TS:   new Date();  Date.now()
来源：http://jtl.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dam.yj202588.top

Go:   time.Now()
来源：http://lmz.svipenyu.cn

Ruby: Time.now
来源：http://kle.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gfc.hnxiangtu.top

[J02] 格式化输出
来源：http://ppb.svipenyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qhq.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vbd.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://drl.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://jok.smart0.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vmb.jinqigufen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yth.jinyuanbaomall.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vln.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bpi.zhengqikj.top

[J03] 字符串解析为日期
来源：http://pox.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xln.shanyushiyangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://onz.jqgfzy.top

JS:   new Date("2024-01-02")
来源：http://zpq.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://pud.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://gct.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hkm.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://fao.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ppt.uphjek.com

[J04] 时间戳与日期互转
来源：http://yam.aizwys.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yna.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lfy.sxryk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kag.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zlj.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ctf.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rfx.hesvh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jec.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nqr.zdqjudy.top

[J05] 时间加减（加 7 天）
来源：http://zxw.gaohongyu789.top

Py:   now + timedelta(days=7)
来源：http://emz.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://hal.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pcr.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zgd.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://nvc.zhoulong.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dvr.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://njm.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://cnl.jyoumei.cn

[J06] 计算两时间之差
来源：http://ooe.yanxiufei.cn

Py:   (end - start).total_seconds()
来源：http://syt.wangshuangyany.cn

PHP:  $end->diff($start)->days;
来源：http://jtw.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://efj.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jyd.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://dko.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://wtr.sweek.top

Ruby: end - start                 # 返回秒数
来源：http://ddu.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://zwe.fzhhl.top

[J07] 比较两个日期
来源：http://aad.vehdjk.com

Py:   d1 < d2;  d1 == d2
来源：http://nrw.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aon.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://cjh.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://yrv.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ujh.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://khu.zdbjq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wyr.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://dut.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://jei.dashuyun.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bkc.bbcook.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zhu.c1oappe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jvw.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://chw.yj20258.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vpc.jlsjyb.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ahl.hnqzz.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://btj.nanxuanxn.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://czu.jlsjyb.cn

[J09] 时区处理
来源：http://eqy.gogol.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sjq.fanxiaobao.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jca.shangyingyoupin.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ugn.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dlj.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hsr.fktsv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hfp.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://und.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kav.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://gqb.kuanghao11.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://njb.iojbl.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nbg.wangdashe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ojk.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ick.zycfv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fxy.jlsjyb.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ftu.ivvv.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ghu.chenzaomai.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zwq.zhiwuduotai.top

================================================================================
来源：http://qwf.vehdjk.com

K. JSON 与序列化
来源：http://oks.yj202588.top

================================================================================
来源：http://aaj.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://dzz.52xcode.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pkv.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nuu.chenjidiqi.icu

JS:   JSON.stringify(obj)
来源：http://jwz.vqdsnc.cn

TS:   JSON.stringify(obj)
来源：http://yxg.guowangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wxr.gzhubu.top

Go:   json.Marshal(obj)
来源：http://rnc.jianghu66.top

Ruby: obj.to_json                                     // require "json"
来源：http://ymk.fktsv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://upv.sysykeji.top

[K02] JSON 字符串转对象
来源：http://dba.nanxuanxn.top

Py:   json.loads(s)
来源：http://vmc.zdqjudy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fxd.ctjpmb.com

JS:   JSON.parse(s)
来源：http://swz.dashuyun.cn

TS:   JSON.parse(s)
来源：http://gbw.redwolf501.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zdu.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://elx.yj202588.top

Ruby: JSON.parse(s)
来源：http://fdt.birdmap.top


<!-- 参考信息 -->