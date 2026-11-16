代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://jhr.tanke756.top

Ruby: def to_s; @name; end
来源：http://xvx.tarul.cn

C#:   public override string ToString() => Name;
来源：http://zhj.jinghuilouyu.cn

[G13] 判断对象类型
来源：http://qcb.tian-w.cn

Py:   isinstance(u, User)
来源：http://ygp.fanxiaobao.xyz

PHP:  $u instanceof User
来源：http://zjq.jianghu66.top

JS:   u instanceof User
来源：http://vju.andypj.xyz

TS:   u instanceof User
来源：http://zlw.shuidangran.top

Java: u instanceof User
来源：http://whw.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://vnr.tarul.cn

Ruby: u.is_a?(User)
来源：http://geu.jinyuanbaomall.cn

C#:   u is User
来源：http://vaq.yj202588.top

[G14] 数据类 / record
来源：http://gjd.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://npd.nwbrower.top

PHP:  // 用 readonly 属性模拟
来源：http://qyb.jinyuanbaomall.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xkv.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://ghx.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://xcc.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://uim.cqqwz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://onu.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://hkv.nwbrower.top

[G15] 枚举
来源：http://lom.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mnz.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sdq.cqqwz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xab.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ehm.jqgufenzy.top

Java: enum Color { RED, GREEN }
来源：http://aev.gotoacloud.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ssd.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://mmr.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://axx.yonumen.top

[G16] 对象转数组 / 字典
来源：http://jaj.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wiw.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://tmg.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://kpc.hnqzz.top

TS:   Object.entries(obj)
来源：http://alt.tanke756.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cwu.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://rjz.gzhubu.top

Ruby: obj.instance_variables
来源：http://swb.jinqigfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://jjj.vehdjk.com

================================================================================
来源：http://hct.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://egh.haohaochexian.top

================================================================================
来源：http://efh.vqdsnc.cn

[H01] try / catch 基础
来源：http://nhs.52xcode.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jlb.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ekt.xingfuxueyuan.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ewe.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lvq.iojbl.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://smf.cqqwz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qcw.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sjt.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://opj.mhx1999.top

[H02] finally / ensure 收尾
来源：http://ehd.dianchejie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tdr.hywenlv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mct.ydjk.org.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ore.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cxg.fengsongda.top

Java: try { f(); } finally { cleanup(); }
来源：http://rzl.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qsv.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://etu.shzxlz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://eum.ppjwa.cn

[H03] 主动抛出异常
来源：http://eqx.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://mih.xylfe.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bms.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://mow.uphjek.com

TS:   throw new Error("错误信息");
来源：http://tuw.zhixingplan.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hmz.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wfq.sweek.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ukb.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://vdz.yuxming.cn

[H04] 自定义异常类型
来源：http://qyc.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://gxz.tian-w.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xst.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://uos.jlsjyb.cn

TS:   class MyError extends Error {}
来源：http://eow.yj202588.top

Java: class MyException extends RuntimeException {}
来源：http://rmp.ywan-chungtsiang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://prw.shuidangran.top

Ruby: class MyError < StandardError; end
来源：http://wgk.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://tad.haohaochexian.top

[H05] 捕获特定类型
来源：http://kwv.fehbvm.com

Py:   except ValueError as e:
来源：http://dhh.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://axj.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://uio.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://buj.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://inh.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ybf.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://gyv.shuidangran.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://acp.mhx1999.top

[H06] 可选值 / 空值安全访问
来源：http://pie.316326.xyz

Py:   value = d.get("k") or default
来源：http://cge.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://doe.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://wja.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rcl.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vqq.daria6918.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ztj.fengsongda.top

Ruby: d&.dig(:a, :b)
来源：http://lfp.yuxming.cn

C#:   obj?.A?.B ?? default
来源：http://mlf.xuetiantiany.cn

[H07] 断言
来源：http://qyu.sjlbkw.cn

Py:   assert x > 0, "必须为正"
来源：http://wfx.316326.xyz

PHP:  assert($x > 0);
来源：http://foz.hammf.cn

JS:   console.assert(x > 0);
来源：http://axb.vehdjk.com

TS:   console.assert(x > 0);
来源：http://rzk.fktsv.cn

Java: assert x > 0 : "必须为正";
来源：http://tku.ywan-chungtsiang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eug.zhoulong.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://edj.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://chh.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://fch.guannengcc.top

Py:   str(e);  traceback.format_exc()
来源：http://hqb.chenlongwang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fjl.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://ytf.gaohongyu789.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vvx.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nbm.hnxiangtu.top

Go:   err.Error()
来源：http://yfz.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://otw.fktsv.cn

C#:   e.Message;  e.StackTrace
来源：http://nyc.ydzc1.top

[H09] 带错误码的异常
来源：http://dwu.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://czt.aibaodan.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jmu.jinqigufen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yin.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lgw.shangyingyoupin.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sdi.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mby.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vqg.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://rhc.c1oappe.top

[H10] 资源自动释放
来源：http://nrl.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://wzd.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nne.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pyi.xingfuxueyuan.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hha.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xbh.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://mro.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ugx.zdbjq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://izx.cucudq.cn

================================================================================
来源：http://qgf.ybcxt.top

I. 正则表达式
来源：http://fnm.shanyushiyangtech.top

================================================================================
来源：http://zxg.ybcxt.top

[I01] 判断是否匹配
来源：http://muk.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mdp.gotoacloud.top

PHP:  preg_match('/\d+/', $s);
来源：http://cly.c1oappe.top

JS:   /\d+/.test(s)
来源：http://fiv.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://csj.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xxw.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nvr.tanke756.top

Ruby: s.match?(/\d+/)
来源：http://wxi.zhaomingkeji.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ecm.vehdjk.com

[I02] 提取所有匹配
来源：http://okw.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://kwk.guowangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yyq.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://odn.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://krp.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://him.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ehm.shuidangran.top

Ruby: s.scan(/\d+/)
来源：http://hoi.gogol.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wjf.cheryme.top

[I03] 提取捕获分组
来源：http://cgn.zdqjudy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pgb.yangfankeji.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pnq.gzhubu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xug.hywenlv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ppp.zhengqikj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pua.bbcook.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sbg.daria6918.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lsx.redwolf501.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xnh.shanyushiyangtech.top

[I04] 正则替换
来源：http://mfx.aizwys.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://txd.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zrj.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tmf.xuetiantiany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dzh.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dxd.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ouw.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hee.chenzaomai.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hpe.dianchejie.cn

[I05] 按正则拆分
来源：http://mgh.xylfe.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uwz.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jii.yanxiufei.cn

JS:   s.split(/\s*,\s*/)
来源：http://dau.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://wzh.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://icx.zdqjudy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rys.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://akj.yj20258888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bdj.redwolf501.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wep.aizwys.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mcu.cheryme.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lep.ydzc1.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hvg.snrcjt.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mnh.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gro.daria6918.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aci.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gwa.yanxiufei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hta.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://bbz.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ava.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uqh.shangyingyoupin.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://atg.jqgfzy.top

TS:   /error/gim
来源：http://vrh.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ikb.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xjm.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://ilm.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://imm.cheryme.top

[I08] 贪婪与非贪婪匹配
来源：http://zcc.vqdsnc.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xrc.jqgufenzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xzf.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vrb.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rhd.jinqigfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://npi.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ldx.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xzc.jyoumei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zbq.fanxiaobao.xyz

================================================================================
来源：http://thv.snrcjt.cn

J. 日期与时间
来源：http://epu.chenlongwang.top

================================================================================
来源：http://kza.fengsongda.top

[J01] 获取当前时间
来源：http://cri.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zrf.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zqe.cucudq.cn

JS:   new Date();  Date.now()
来源：http://hfc.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://jqb.sweek.top

Java: LocalDateTime.now();  Instant.now()
来源：http://emd.zhoulong.xyz

Go:   time.Now()
来源：http://nax.jinqigufen.top

Ruby: Time.now
来源：http://dfd.jqgufenzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oqe.xingfuxueyuan.xyz

[J02] 格式化输出
来源：http://oma.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qnk.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sje.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xcn.sweek.top

TS:   d.toISOString()
来源：http://pwl.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://alu.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dsd.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rxp.nwbrower.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://udr.316326.xyz

[J03] 字符串解析为日期
来源：http://fad.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fyx.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dnp.vehdjk.com

JS:   new Date("2024-01-02")
来源：http://fbw.ehwqpu.com

TS:   new Date("2024-01-02")
来源：http://ezs.shanyushiyangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://uwt.meibo888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ldi.xziqi.cn

Ruby: Date.parse("2024-01-02")
来源：http://rle.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://izx.sjlbkw.cn

[J04] 时间戳与日期互转
来源：http://jsn.quarkkingdee.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://esv.snrcjt.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fzn.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kdh.svipenyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sky.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mbx.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pyy.daria6918.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ywt.aizwys.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qsq.ydzc1.top

[J05] 时间加减（加 7 天）
来源：http://lqo.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://eoh.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rej.yj20258888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ivg.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xfi.ydjk.org.cn

Java: LocalDate.now().plusDays(7)
来源：http://bbo.ybcxt.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mcd.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://xtb.aibaodan.cn

C#:   DateTime.Now.AddDays(7)
来源：http://acj.ivvv.top

[J06] 计算两时间之差
来源：http://aps.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://ybr.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://vph.cqqwz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iad.dianchejie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qde.jlsjyb.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yvl.hnqzz.top

Go:   end.Sub(start).Hours()
来源：http://wzr.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://ooe.dashuyun.cn

C#:   (end - start).TotalSeconds
来源：http://rqv.yangfankeji.com

[J07] 比较两个日期
来源：http://bdj.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://fey.zhijiandao.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mdd.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://ahf.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://top.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mfa.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://orn.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://zvp.xinyue.icu

C#:   d1 < d2;  d1 == d2
来源：http://aof.jinqigfzy.top

[J08] 提取年月日与星期
来源：http://rbe.daxiang520.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nfi.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jyo.jyoumei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lmw.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dsl.hfpthk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://euu.snrcjt.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ukr.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hdr.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vww.fzhhl.top

[J09] 时区处理
来源：http://tjz.hesvh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kuh.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rfw.9152youxi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bvl.hywenlv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aqu.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nki.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ygw.xinyue.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://uyt.nanxinkj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://itf.quarkkingdee.top

[J10] 取今天 / 本月第一天
来源：http://txc.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://irh.ybcxt.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lkt.svipenyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://luj.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qqt.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uuh.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ejn.smart0.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ppa.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wak.andypj.xyz


<!-- 参考信息 -->