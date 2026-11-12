代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wma.ctjpmb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://anj.uphjek.com

Java: enum Color { RED, GREEN }
来源：http://usr.shangyingyoupin.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ekc.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://ebf.zdbjq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ofm.zhongyouzk.top

[G16] 对象转数组 / 字典
来源：http://wkz.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uzc.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://feq.zycfv.cn

JS:   Object.entries(obj)
来源：http://qzz.ppjwa.cn

TS:   Object.entries(obj)
来源：http://auw.feifeiyinyue.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aut.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uyw.bjfxy.top

Ruby: obj.instance_variables
来源：http://nyz.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://zvc.tianlin.xyz

================================================================================
来源：http://pzr.zhengqikj.top

H. 异常与错误处理
来源：http://upz.hywenlv.cn

================================================================================
来源：http://abs.hnxiangtu.top

[H01] try / catch 基础
来源：http://gkv.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nwn.jinyuanbaomall.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bqs.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dii.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vbv.0kj1m.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hwr.dianchejie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ajj.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rwa.yueranfly.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gkh.cheryme.top

[H02] finally / ensure 收尾
来源：http://amn.feifeiyinyue.top

Py:   try: f()⏎finally: cleanup()
来源：http://xgn.hywenlv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lya.haohaochexian.top

JS:   try { f(); } finally { cleanup(); }
来源：http://eqv.sysykeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rna.fengsongda.top

Java: try { f(); } finally { cleanup(); }
来源：http://ldx.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sep.xylfe.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xhv.jiagoushi.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://quf.zhongyouzk.top

[H03] 主动抛出异常
来源：http://qga.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://ibj.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://luq.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://tjd.yj202588.top

TS:   throw new Error("错误信息");
来源：http://oqm.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://brw.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bew.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xxw.zhengqikj.top

C#:   throw new ArgumentException("错误信息");
来源：http://yli.zhijiandao.cn

[H04] 自定义异常类型
来源：http://edw.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://lco.ivvv.top

PHP:  class MyError extends RuntimeException {}
来源：http://aeo.epnwcf.com

JS:   class MyError extends Error {}
来源：http://rgv.fzhhl.top

TS:   class MyError extends Error {}
来源：http://ybl.zhongyouzk.top

Java: class MyException extends RuntimeException {}
来源：http://gkh.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ybr.hesvh.cn

Ruby: class MyError < StandardError; end
来源：http://bil.jiagoushi.top

C#:   class MyException : Exception {}
来源：http://eqv.guowangkeji.top

[H05] 捕获特定类型
来源：http://der.fengsongda.top

Py:   except ValueError as e:
来源：http://tnk.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cci.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://bfb.hywenlv.cn

TS:   if (e instanceof TypeError) {}
来源：http://zlp.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://vbs.yongpay.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zgm.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://prm.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zyy.xziqi.cn

[H06] 可选值 / 空值安全访问
来源：http://psl.aizwys.cn

Py:   value = d.get("k") or default
来源：http://uez.jiagoushi.top

PHP:  $v = $d["k"] ?? null;
来源：http://log.xuanzx.com

JS:   obj?.a?.b;  d ?? default
来源：http://psf.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://agm.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bnr.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://saj.cqqwz.cn

Ruby: d&.dig(:a, :b)
来源：http://ufw.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://del.tian-w.cn

[H07] 断言
来源：http://avn.vqdsnc.cn

Py:   assert x > 0, "必须为正"
来源：http://sib.hcnkem.com

PHP:  assert($x > 0);
来源：http://krr.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://qag.guowangkeji.top

TS:   console.assert(x > 0);
来源：http://nbd.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://hlu.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bge.ehwqpu.com

Ruby: raise "必须为正" unless x > 0
来源：http://abr.ppjwa.cn

C#:   Debug.Assert(x > 0);
来源：http://gkj.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://vqv.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://iul.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fnz.cashguo.top

JS:   e.message;  e.stack
来源：http://jxn.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yed.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vre.52xcode.cn

Go:   err.Error()
来源：http://qfl.zhaomingkeji.xyz

Ruby: e.message;  e.backtrace
来源：http://ple.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://jmy.hcnkem.com

[H09] 带错误码的异常
来源：http://zlv.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hdk.shangyingyoupin.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://plq.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tbl.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://urx.havefunace.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nbd.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://joc.zhengqikj.top

Ruby: raise MyError.new("fail", 500)
来源：http://qcd.meibo888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zvu.daxiang520.top

[H10] 资源自动释放
来源：http://ocz.quarkkingdee.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://amz.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vpc.sjlbkw.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nah.sufxvd.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ldw.zhaomingkeji.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gzq.yongpay.top

Go:   defer f.Close()
来源：http://ybk.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fbo.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hvg.jinqigfzy.top

================================================================================
来源：http://luy.xinyue.icu

I. 正则表达式
来源：http://kcp.ehwqpu.com

================================================================================
来源：http://qsi.vqdsnc.cn

[I01] 判断是否匹配
来源：http://pwv.vqdsnc.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jhb.daxiang520.top

PHP:  preg_match('/\d+/', $s);
来源：http://evl.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://tdu.ctjpmb.com

TS:   /\d+/.test(s)
来源：http://chy.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uhs.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wnn.meibo888.top

Ruby: s.match?(/\d+/)
来源：http://bon.chenjidiqi.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tan.sufxvd.cn

[I02] 提取所有匹配
来源：http://efo.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://png.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xtk.wangdashe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ypc.shzxlz.cn

TS:   s.match(/\d+/g)
来源：http://rja.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://plb.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cus.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://nss.bjfxy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jqp.fktsv.cn

[I03] 提取捕获分组
来源：http://zna.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kia.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vdu.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fvv.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kof.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://utq.bbcook.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vhh.guannengcc.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kjd.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zlt.cucudq.cn

[I04] 正则替换
来源：http://eyw.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ltc.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dzb.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ddo.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://gwn.yuanzhike.top

Java: s.replaceAll("\\d+", "#")
来源：http://yqm.sjlbkw.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yrf.zdqjudy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wnk.ppjwa.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://szd.bjfxy.top

[I05] 按正则拆分
来源：http://uqo.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://doo.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lnt.hammf.cn

JS:   s.split(/\s*,\s*/)
来源：http://vyy.zhengqikj.top

TS:   s.split(/\s*,\s*/)
来源：http://fgn.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://rdi.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rge.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hqb.pycfn.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cjc.pengpengdd.cyou

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://anw.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tyu.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://phh.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gbg.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xao.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zwx.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://amp.ybcxt.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://suf.316326.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eez.yj202588.top

[I07] 忽略大小写与多行模式
来源：http://jlf.yangfankeji.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vxh.vehdjk.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zda.ehwqpu.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://atc.sufxvd.cn

TS:   /error/gim
来源：http://ion.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://htv.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://usb.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://pvc.316326.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wce.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://flg.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lap.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ngm.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://een.nwbrower.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qdx.hysaishi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://idi.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pdv.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ctx.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oud.fengsongda.top

================================================================================
来源：http://xdc.epnwcf.com

J. 日期与时间
来源：http://ufs.shanyushiyangtech.top

================================================================================
来源：http://zfi.chenlongwang.top

[J01] 获取当前时间
来源：http://eld.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pfb.vqdsnc.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://usf.zhongyouzk.top

JS:   new Date();  Date.now()
来源：http://azi.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://pky.zhiwuduotai.top

Java: LocalDateTime.now();  Instant.now()
来源：http://oxp.wangshuangyany.cn

Go:   time.Now()
来源：http://vfb.epnwcf.com

Ruby: Time.now
来源：http://ngm.chenzaomai.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uuj.andypj.xyz

[J02] 格式化输出
来源：http://qbt.yuanzhike.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://orx.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://epr.snrcjt.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fvy.yfazqb.com

TS:   d.toISOString()
来源：http://nie.tarul.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fuo.xylfe.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qpr.zdqjudy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mlp.pycfn.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://asq.vqdsnc.cn

[J03] 字符串解析为日期
来源：http://szp.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zyh.zhengqikj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gvv.nanxinkj.top

JS:   new Date("2024-01-02")
来源：http://ngn.fzhhl.top

TS:   new Date("2024-01-02")
来源：http://sqa.chenzaomai.com

Java: LocalDate.parse("2024-01-02")
来源：http://hga.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dkl.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://lhj.xinyue.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vvg.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://fof.hammf.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zrh.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://omf.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zgg.nanxinkj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://oah.yuxming.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iph.daria6918.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dsq.zhixingplan.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://onr.hywenlv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://teb.cheryme.top

[J05] 时间加减（加 7 天）
来源：http://yvt.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://eig.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://nia.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://flt.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vwx.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://dhh.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sgt.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://glz.guannengcc.top

C#:   DateTime.Now.AddDays(7)
来源：http://tts.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://wnd.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://bqj.yangfankeji.com

PHP:  $end->diff($start)->days;
来源：http://tbf.xinyue.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zjc.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ucw.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://mhc.sweek.top

Go:   end.Sub(start).Hours()
来源：http://gas.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://kus.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://mla.yj20258888.top

[J07] 比较两个日期
来源：http://wjl.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://fyd.yonumen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nuh.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://obm.xuanzx.com

TS:   d1.getTime() < d2.getTime()
来源：http://oyt.shanyushiyangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tbi.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://api.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://wle.jinqigufen.top

C#:   d1 < d2;  d1 == d2
来源：http://flz.hcnkem.com

[J08] 提取年月日与星期
来源：http://mbq.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oli.zhongyouzk.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zae.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wod.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fjs.xinyue.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://spk.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vee.jqgfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oph.yj20258888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zkj.ydjk.org.cn

[J09] 时区处理
来源：http://nlh.jqgfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pje.gzhubu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mlr.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vgb.9152youxi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wua.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ant.xingfuxueyuan.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xfa.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rdd.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qgu.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://bxy.smart0.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://ytc.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://onv.hesvh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tqp.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ldx.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yqb.sweek.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xdz.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jnn.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vcu.fehbvm.com

================================================================================
来源：http://bpn.shanyushiyangtech.top

K. JSON 与序列化
来源：http://cja.aizwys.cn

================================================================================
来源：http://aqq.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://dnw.cucudq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://utn.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uxu.quarkkingdee.top

JS:   JSON.stringify(obj)
来源：http://lfu.guowangkeji.top

TS:   JSON.stringify(obj)
来源：http://fqy.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://trt.aizwys.cn

Go:   json.Marshal(obj)
来源：http://lla.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tio.nwbrower.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kci.havefunace.top

[K02] JSON 字符串转对象
来源：http://hwc.gaohongyu789.top

Py:   json.loads(s)
来源：http://eil.zhengqikj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lle.shanyushiyangtech.top

JS:   JSON.parse(s)
来源：http://kgv.wangdashe.top

TS:   JSON.parse(s)
来源：http://bhd.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qkj.sysykeji.top

Go:   json.Unmarshal(data, &v)
来源：http://lsc.jiagoushi.top

Ruby: JSON.parse(s)
来源：http://bat.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nlu.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://pyz.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ogm.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://abs.sysykeji.top


<!-- 参考信息 -->