代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://xma.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://lyd.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://qfg.yangfankeji.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ces.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://kwy.shzxlz.cn

[G15] 枚举
来源：http://skv.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zep.hysaishi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lzi.ywan-chungtsiang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qzx.zdqjudy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kod.uphjek.com

Java: enum Color { RED, GREEN }
来源：http://igd.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jsp.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://fye.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xdg.ydzc1.top

[G16] 对象转数组 / 字典
来源：http://lgb.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ybp.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://bzi.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://xeo.yueranfly.top

TS:   Object.entries(obj)
来源：http://oem.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xpq.shangyingyoupin.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gfq.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://pos.xingfuxueyuan.xyz

C#:   // 用反射或 System.Text.Json
来源：http://hmi.hywenlv.cn

================================================================================
来源：http://bvk.mhx1999.top

H. 异常与错误处理
来源：http://jcd.xuetiantiany.cn

================================================================================
来源：http://bbd.jianghu66.top

[H01] try / catch 基础
来源：http://ykd.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://flv.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cuh.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xrc.bbcook.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ysr.xinyue.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kis.yuanzhike.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nmt.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nyx.yueranfly.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eko.bbcook.cn

[H02] finally / ensure 收尾
来源：http://egw.aizwys.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vef.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cim.jinqigfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dsp.jinghuilouyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rro.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://xvz.yj202588.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nuj.xuanzx.com

Ruby: begin; f; ensure; cleanup; end
来源：http://vxy.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lqv.tian-w.cn

[H03] 主动抛出异常
来源：http://ose.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://jvc.zdqjudy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kqz.xuanzx.com

JS:   throw new Error("错误信息");
来源：http://msn.xingfuxueyuan.xyz

TS:   throw new Error("错误信息");
来源：http://gim.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://twl.xylfe.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vxs.zhixingplan.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bod.316326.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://dtp.andypj.xyz

[H04] 自定义异常类型
来源：http://yil.fzhhl.top

Py:   class MyError(Exception): pass
来源：http://vuz.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://cfu.tianlin.xyz

JS:   class MyError extends Error {}
来源：http://jae.fengsongda.top

TS:   class MyError extends Error {}
来源：http://eua.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://aji.guowangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gmd.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://jnb.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://ojq.yj202588.top

[H05] 捕获特定类型
来源：http://dzm.zdbjq.cn

Py:   except ValueError as e:
来源：http://yqe.jyoumei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jii.uphjek.com

JS:   if (e instanceof TypeError) {}
来源：http://quf.yongpay.top

TS:   if (e instanceof TypeError) {}
来源：http://ecw.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://jcg.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sdg.wangdashe.top

Ruby: rescue ArgumentError => e
来源：http://txu.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tuv.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://qds.ydzc1.top

Py:   value = d.get("k") or default
来源：http://dsn.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://nmg.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kpe.fehbvm.com

TS:   obj?.a?.b;  d ?? default
来源：http://udk.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zhc.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ngb.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://qfl.aizwys.cn

C#:   obj?.A?.B ?? default
来源：http://ojo.yanxiufei.cn

[H07] 断言
来源：http://ndn.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://dod.shuidangran.top

PHP:  assert($x > 0);
来源：http://jqr.xziqi.cn

JS:   console.assert(x > 0);
来源：http://nhe.tanke756.top

TS:   console.assert(x > 0);
来源：http://gvg.tianlin.xyz

Java: assert x > 0 : "必须为正";
来源：http://fxa.hammf.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rno.jyoumei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yao.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://hvq.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://del.dashuyun.cn

Py:   str(e);  traceback.format_exc()
来源：http://rie.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gsg.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://fnq.zhongyouzk.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fez.guannengcc.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uaj.cucudq.cn

Go:   err.Error()
来源：http://vxq.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://uiz.jyoumei.cn

C#:   e.Message;  e.StackTrace
来源：http://ntf.shuidangran.top

[H09] 带错误码的异常
来源：http://wqd.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uae.hesvh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vma.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pps.ehwqpu.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kjd.yangfankeji.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qco.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ghx.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://qxz.guowangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qtf.ydjk.org.cn

[H10] 资源自动释放
来源：http://wsy.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nzn.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hyd.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://boa.fanxiaobao.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dbb.jqgfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wdr.daria6918.cn

Go:   defer f.Close()
来源：http://kji.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rrx.hywenlv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qbb.bjfxy.top

================================================================================
来源：http://eje.jianghu66.top

I. 正则表达式
来源：http://xuf.gzhubu.top

================================================================================
来源：http://jrq.zdqjudy.top

[I01] 判断是否匹配
来源：http://afp.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zkb.dashuyun.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gdf.ywan-chungtsiang.top

JS:   /\d+/.test(s)
来源：http://cgm.sxryk.cn

TS:   /\d+/.test(s)
来源：http://gry.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wys.xylfe.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zmv.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://igj.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dsc.daria6918.cn

[I02] 提取所有匹配
来源：http://yfx.ctjpmb.com

Py:   re.findall(r"\d+", s)
来源：http://hau.gzhubu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sqf.hysaishi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vkw.ywan-chungtsiang.top

TS:   s.match(/\d+/g)
来源：http://mfy.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gfx.yvedp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kci.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://npx.yvedp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tqs.shzxlz.cn

[I03] 提取捕获分组
来源：http://snh.cucudq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rqo.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hhf.jiagoushi.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aio.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fhe.dashuyun.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nkv.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://toz.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ayh.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yml.jyoumei.cn

[I04] 正则替换
来源：http://tge.xziqi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://crd.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pid.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://ggg.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kxq.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://poj.shanyushiyangtech.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dxz.svipenyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fit.zhijiandao.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://him.yangfankeji.com

[I05] 按正则拆分
来源：http://rmq.guowangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ole.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gyo.xziqi.cn

JS:   s.split(/\s*,\s*/)
来源：http://mjl.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://leo.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://evz.ppjwa.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ocw.guannengcc.top

Ruby: s.split(/\s*,\s*/)
来源：http://aqn.ctjpmb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ryy.ctjpmb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cek.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bxq.dianchejie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ial.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tuu.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oee.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ydl.shanyushiyangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://umb.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pnr.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://izl.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://ssh.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ioc.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yky.ehwqpu.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ozr.shzxlz.cn

TS:   /error/gim
来源：http://uav.jianghu66.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://thm.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cpz.hnxiangtu.top

Ruby: s.scan(/error/i)
来源：http://bnx.zhiwuduotai.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kex.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://rxn.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://clf.zhijiandao.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lkm.dianchejie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://beq.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://clf.yfazqb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://btj.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://joy.jinqigfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fnl.fzhhl.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://njx.uphjek.com

================================================================================
来源：http://fpu.yvedp.cn

J. 日期与时间
来源：http://lqq.shzxlz.cn

================================================================================
来源：http://ezy.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://oyu.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://odf.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://avr.fktsv.cn

JS:   new Date();  Date.now()
来源：http://ehb.gaohongyu789.top

TS:   new Date();  Date.now()
来源：http://zkf.feifeiyinyue.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hwy.ehwqpu.com

Go:   time.Now()
来源：http://zdc.hfpthk.cn

Ruby: Time.now
来源：http://blk.shuidangran.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hgv.sweek.top

[J02] 格式化输出
来源：http://nlq.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ati.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ooy.vehdjk.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://irz.vqdsnc.cn

TS:   d.toISOString()
来源：http://kzs.ctjpmb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hdg.chenlongwang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kzj.birdmap.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://imu.ybcxt.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gfk.yfazqb.com

[J03] 字符串解析为日期
来源：http://xeh.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://htb.xinyue.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sgk.dashuyun.cn

JS:   new Date("2024-01-02")
来源：http://dyk.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://rrp.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://zba.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xqj.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://ygu.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uoa.yuxming.cn

[J04] 时间戳与日期互转
来源：http://mhp.sjlbkw.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nwv.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://swr.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://toj.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fgl.xingfuxueyuan.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tay.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gan.fengsongda.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rsn.hfpthk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fxg.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://adr.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://gkh.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kvd.zhaomingkeji.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uga.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gyx.zhaomingkeji.xyz

Java: LocalDate.now().plusDays(7)
来源：http://kvn.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://klx.jinyuanbaomall.cn

Ruby: Time.now + 7 * 86400
来源：http://gxf.bbcook.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kvy.tarul.cn

[J06] 计算两时间之差
来源：http://hgy.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://juv.yueranfly.top

PHP:  $end->diff($start)->days;
来源：http://xsh.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fov.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nnj.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://flu.c1oappe.top

Go:   end.Sub(start).Hours()
来源：http://gsh.tianlin.xyz

Ruby: end - start                 # 返回秒数
来源：http://mdv.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://xmx.cashguo.top

[J07] 比较两个日期
来源：http://nci.svipenyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://fvt.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aok.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://meo.xuetiantiany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://evs.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vjj.vqdsnc.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vya.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://olz.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://zju.sweek.top

[J08] 提取年月日与星期
来源：http://iyg.vqdsnc.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://brm.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://auy.gzhubu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vtc.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fhd.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jne.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pcj.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qws.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bfr.yfazqb.com

[J09] 时区处理
来源：http://cgv.bbcook.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gyw.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lpt.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wsd.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wwg.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bcy.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uee.fzhhl.top

Ruby: Time.now.getlocal("+08:00")
来源：http://snf.guowangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ybv.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://eri.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://grq.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://via.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nei.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uwn.jianghu66.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ywm.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://krc.zdbjq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fso.shanyushiyangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vgt.chenzaomai.com

================================================================================
来源：http://kja.shanyushiyangtech.top

K. JSON 与序列化
来源：http://hov.sxryk.cn

================================================================================
来源：http://mwm.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://vah.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sre.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pvg.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://xga.fktsv.cn

TS:   JSON.stringify(obj)
来源：http://xjr.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mlq.nwbrower.top

Go:   json.Marshal(obj)
来源：http://izo.pengpengdd.cyou

Ruby: obj.to_json                                     // require "json"
来源：http://qup.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xfi.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://pes.52xcode.cn

Py:   json.loads(s)
来源：http://uqc.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nna.jiagoushi.top

JS:   JSON.parse(s)
来源：http://dxj.yfazqb.com


<!-- 参考信息 -->