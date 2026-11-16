代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://pvu.svipenyu.cn

JS:   toString() { return this.name; }
来源：http://sww.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://lyj.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://deb.yfazqb.com

Go:   func (u User) String() string { return u.Name }
来源：http://mvh.mhx1999.top

Ruby: def to_s; @name; end
来源：http://vkr.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://jpo.bjfxy.top

[G13] 判断对象类型
来源：http://ecq.quarkkingdee.top

Py:   isinstance(u, User)
来源：http://csm.sjlbkw.cn

PHP:  $u instanceof User
来源：http://dqx.jiagoushi.top

JS:   u instanceof User
来源：http://jww.nwbrower.top

TS:   u instanceof User
来源：http://obt.yj202588.top

Java: u instanceof User
来源：http://mgk.jianghu66.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mck.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://rgj.fanxiaobao.xyz

C#:   u is User
来源：http://nvu.zdqjudy.top

[G14] 数据类 / record
来源：http://nhm.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vnl.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://anq.xylfe.cn

JS:   // 无内置：普通类或对象字面量
来源：http://csj.0kj1m.cn

TS:   type User = { name: string; age: number };
来源：http://vis.hfpthk.cn

Java: record User(String name, int age) {}
来源：http://iuc.birdmap.top

Go:   type User struct { Name string; Age int }
来源：http://abv.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fzl.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://rcc.jinyuanbaomall.cn

[G15] 枚举
来源：http://hcq.jqgfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ukb.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wnx.dashuyun.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zbo.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zdt.pycfn.com

Java: enum Color { RED, GREEN }
来源：http://zni.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ned.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://ovp.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gga.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://nff.yonumen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eag.jinqigfzy.top

PHP:  get_object_vars($obj);
来源：http://jci.hfpthk.cn

JS:   Object.entries(obj)
来源：http://fhv.jiagoushi.top

TS:   Object.entries(obj)
来源：http://fkj.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iqy.birdmap.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tss.bbcook.cn

Ruby: obj.instance_variables
来源：http://nah.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://gzc.sysykeji.top

================================================================================
来源：http://coo.fanxiaobao.xyz

H. 异常与错误处理
来源：http://twd.chenjidiqi.icu

================================================================================
来源：http://vsp.xylfe.cn

[H01] try / catch 基础
来源：http://gcl.9152youxi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ynu.jinqigufen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sjr.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yrs.gotoacloud.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ktc.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dpr.ehwqpu.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aji.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cpq.jinqigufen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hxg.smart0.xyz

[H02] finally / ensure 收尾
来源：http://iyj.yfazqb.com

Py:   try: f()⏎finally: cleanup()
来源：http://qjq.ywan-chungtsiang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qzh.xuetiantiany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tbp.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://riu.birdmap.top

Java: try { f(); } finally { cleanup(); }
来源：http://vho.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jsy.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://isr.yongpay.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lwc.yuxming.cn

[H03] 主动抛出异常
来源：http://iay.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://eva.hywenlv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bmw.hesvh.cn

JS:   throw new Error("错误信息");
来源：http://hrr.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://rmu.yvedp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iwq.wangdashe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aha.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ibl.hywenlv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://reg.pengpengdd.cyou

[H04] 自定义异常类型
来源：http://npm.mhx1999.top

Py:   class MyError(Exception): pass
来源：http://wqs.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://owc.daxiang520.top

JS:   class MyError extends Error {}
来源：http://duc.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://evf.cdnleiting.top

Java: class MyException extends RuntimeException {}
来源：http://tyr.yuxming.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lmt.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://esc.birdmap.top

C#:   class MyException : Exception {}
来源：http://vht.yuanzhike.top

[H05] 捕获特定类型
来源：http://blz.nanxinkj.top

Py:   except ValueError as e:
来源：http://xgn.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gjz.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://xrc.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://rpd.fzhhl.top

Java: catch (IOException | SQLException e) {}
来源：http://czu.jinqigufen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jfd.nanxuanxn.top

Ruby: rescue ArgumentError => e
来源：http://prh.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://imy.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://zfa.hnqzz.top

Py:   value = d.get("k") or default
来源：http://lxj.birdmap.top

PHP:  $v = $d["k"] ?? null;
来源：http://bcv.shangyingyoupin.top

JS:   obj?.a?.b;  d ?? default
来源：http://vaf.yj20258.top

TS:   obj?.a?.b;  d ?? default
来源：http://ukq.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ore.yanxiufei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://iez.jinqigfzy.top

Ruby: d&.dig(:a, :b)
来源：http://rjp.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://atb.gaohongyu789.top

[H07] 断言
来源：http://lmb.zhoulong.xyz

Py:   assert x > 0, "必须为正"
来源：http://rfi.yonumen.top

PHP:  assert($x > 0);
来源：http://jdo.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://cpa.andypj.xyz

TS:   console.assert(x > 0);
来源：http://kfx.xylfe.cn

Java: assert x > 0 : "必须为正";
来源：http://zgc.xziqi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wie.ehwqpu.com

Ruby: raise "必须为正" unless x > 0
来源：http://ajd.redwolf501.top

C#:   Debug.Assert(x > 0);
来源：http://ijt.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://vdx.gotoacloud.top

Py:   str(e);  traceback.format_exc()
来源：http://ifi.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bkv.9152youxi.cn

JS:   e.message;  e.stack
来源：http://kpb.snrcjt.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rva.sweek.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ouo.fengsongda.top

Go:   err.Error()
来源：http://sct.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://csh.fzhhl.top

C#:   e.Message;  e.StackTrace
来源：http://dji.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://nyy.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aqi.zdbjq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bug.yuxming.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iqw.haohaochexian.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qny.ctjpmb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dpd.zycfv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nlf.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://yza.jlsjyb.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fqi.haohaochexian.top

[H10] 资源自动释放
来源：http://cpo.ivvv.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://uvt.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zlt.jinghuilouyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ahl.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fuo.ydzc1.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lxv.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://him.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lse.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pkw.xinyue.icu

================================================================================
来源：http://skr.tian-w.cn

I. 正则表达式
来源：http://ajo.fehbvm.com

================================================================================
来源：http://rgc.pengpengdd.cyou

[I01] 判断是否匹配
来源：http://bmr.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oto.jqgufenzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://slk.yvedp.cn

JS:   /\d+/.test(s)
来源：http://lyp.xuetiantiany.cn

TS:   /\d+/.test(s)
来源：http://bdc.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ren.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://roo.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://snk.yuanzhike.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lzm.xinyue.icu

[I02] 提取所有匹配
来源：http://etg.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://qlk.tianlin.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cxv.tarul.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fii.shuidangran.top

TS:   s.match(/\d+/g)
来源：http://piy.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ehj.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aoa.hongshengwenyu.top

Ruby: s.scan(/\d+/)
来源：http://uel.zhixingplan.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ivl.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://rsp.zdbjq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wuh.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yyj.fzhhl.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ywh.nanxinkj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://swf.jiagoushi.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://khc.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wjj.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://toy.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vnz.bjfxy.top

[I04] 正则替换
来源：http://cii.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wwm.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qhv.svipenyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://blw.gzhubu.top

TS:   s.replace(/\d+/g, "#")
来源：http://jwn.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://him.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://win.hysaishi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://adg.ydjk.org.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sdz.zhiwuduotai.top

[I05] 按正则拆分
来源：http://fhq.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lvb.hesvh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fpc.shanyushiyangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://rwq.ctjpmb.com

TS:   s.split(/\s*,\s*/)
来源：http://gkr.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://zng.kuanghao11.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://arw.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://trp.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yuw.jiagoushi.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dny.xingfuxueyuan.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hpj.zdbjq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kwy.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wvo.jianghu66.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xeq.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://etl.zycfv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vln.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ssj.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nmk.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://gym.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cca.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://obo.jlsjyb.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://inv.guowangkeji.top

TS:   /error/gim
来源：http://qhw.snrcjt.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ezh.cheryme.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://khi.sjlbkw.cn

Ruby: s.scan(/error/i)
来源：http://nmt.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zlr.tanke756.top

[I08] 贪婪与非贪婪匹配
来源：http://qjx.chenlongwang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qax.ivvv.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://avf.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lcd.kuanghao11.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ovq.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://rtu.dashuyun.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://smt.xylfe.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oat.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yek.jqgfzy.top

================================================================================
来源：http://hkr.yj20258888.top

J. 日期与时间
来源：http://oyj.hnqzz.top

================================================================================
来源：http://pwu.hesvh.cn

[J01] 获取当前时间
来源：http://sib.bbcook.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://blv.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vto.gogol.net.cn

JS:   new Date();  Date.now()
来源：http://snp.aizwys.cn

TS:   new Date();  Date.now()
来源：http://akr.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://crb.tanke756.top

Go:   time.Now()
来源：http://sxc.shanyushiyangtech.top

Ruby: Time.now
来源：http://xrh.tanke756.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nvn.tanke756.top

[J02] 格式化输出
来源：http://jjz.zhiwuduotai.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://omb.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eev.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ymg.zhoulong.xyz

TS:   d.toISOString()
来源：http://zid.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fsy.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dpg.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xic.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mok.guannengcc.top

[J03] 字符串解析为日期
来源：http://yce.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qwc.ctjpmb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sqv.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://kvj.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://xvi.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ocj.hfpthk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ytc.dianchejie.cn

Ruby: Date.parse("2024-01-02")
来源：http://xfw.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yio.yj20258.top

[J04] 时间戳与日期互转
来源：http://vya.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iav.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qfw.jinqigufen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yvu.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lwt.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cvq.0kj1m.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xwf.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vra.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iuw.c1oappe.top

[J05] 时间加减（加 7 天）
来源：http://qqo.xuetiantiany.cn

Py:   now + timedelta(days=7)
来源：http://eqx.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tgr.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kva.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rnk.fengsongda.top

Java: LocalDate.now().plusDays(7)
来源：http://sif.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xjd.hcnkem.com

Ruby: Time.now + 7 * 86400
来源：http://lvs.tarul.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iya.xuanzx.com

[J06] 计算两时间之差
来源：http://slm.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://zve.ydzc1.top

PHP:  $end->diff($start)->days;
来源：http://bgz.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://azn.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cti.jqgufenzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://qej.shanyushiyangkeji.top

Go:   end.Sub(start).Hours()
来源：http://cxd.vqdsnc.cn

Ruby: end - start                 # 返回秒数
来源：http://siz.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://jgp.havefunace.top

[J07] 比较两个日期
来源：http://ygb.iojbl.cn

Py:   d1 < d2;  d1 == d2
来源：http://fpm.nwbrower.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xwu.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://cll.daxiang520.top

TS:   d1.getTime() < d2.getTime()
来源：http://yrg.chenzaomai.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vjg.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eug.andypj.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://mql.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://dms.hcnkem.com

[J08] 提取年月日与星期
来源：http://fmh.aizwys.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xep.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jqv.jinqigfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://neg.chenlongwang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vxs.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ilh.jinghuilouyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pzx.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jms.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://reh.redwolf501.top

[J09] 时区处理
来源：http://dzu.52xcode.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gxk.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mvm.zhoulong.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gxy.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lqn.ctjpmb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gmw.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iyn.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yri.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fte.sweek.top

[J10] 取今天 / 本月第一天
来源：http://uya.guannengcc.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fnq.xuetiantiany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oes.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eav.hesvh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://igc.nanxuanxn.top


<!-- 参考信息 -->