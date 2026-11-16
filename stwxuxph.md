代发 wailian999

C#:   public / protected / private / internal
来源：http://quz.quarkkingdee.top

[G11] getter / setter
来源：http://pfw.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://unq.cashguo.top

PHP:  public function getName(): string { return $this->name; }
来源：http://epw.uphjek.com

JS:   get name() { return this._name; }
来源：http://qaa.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://iam.zdqjudy.top

Java: public String getName() { return name; }
来源：http://ygl.tarul.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://stm.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://jil.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://syd.sjlbkw.cn

[G12] 对象转字符串
来源：http://adh.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://fzk.bjfxy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://grk.ehwqpu.com

JS:   toString() { return this.name; }
来源：http://isw.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://iyg.svipenyu.cn

Java: @Override public String toString() { return name; }
来源：http://yhj.daria6918.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dqx.cashguo.top

Ruby: def to_s; @name; end
来源：http://upb.ydzc1.top

C#:   public override string ToString() => Name;
来源：http://psw.sufxvd.cn

[G13] 判断对象类型
来源：http://rtz.cqqwz.cn

Py:   isinstance(u, User)
来源：http://leu.bbcook.cn

PHP:  $u instanceof User
来源：http://uxi.epnwcf.com

JS:   u instanceof User
来源：http://gmz.svipenyu.cn

TS:   u instanceof User
来源：http://nti.zhoulong.xyz

Java: u instanceof User
来源：http://jdw.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ylz.yfazqb.com

Ruby: u.is_a?(User)
来源：http://akt.hesvh.cn

C#:   u is User
来源：http://ydt.gzhubu.top

[G14] 数据类 / record
来源：http://sjq.yangfankeji.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mnm.xuanzx.com

PHP:  // 用 readonly 属性模拟
来源：http://hfx.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://ifz.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://vql.9152youxi.cn

Java: record User(String name, int age) {}
来源：http://ovg.guowangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://vwf.ehwqpu.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://txa.zhoulong.xyz

C#:   record User(string Name, int Age);
来源：http://ddf.zhaomingkeji.xyz

[G15] 枚举
来源：http://okx.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lyp.ppjwa.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ccv.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vcg.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dnt.c1oappe.top

Java: enum Color { RED, GREEN }
来源：http://jnh.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sbf.jinghuilouyu.cn

Ruby: Color = %i[red green].freeze
来源：http://zsw.yuxming.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oiw.cdnleiting.top

[G16] 对象转数组 / 字典
来源：http://wev.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gcy.shanyushiyangtech.top

PHP:  get_object_vars($obj);
来源：http://wrm.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://kgy.sufxvd.cn

TS:   Object.entries(obj)
来源：http://eye.zhengqikj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sej.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cbf.redwolf501.top

Ruby: obj.instance_variables
来源：http://pod.nwbrower.top

C#:   // 用反射或 System.Text.Json
来源：http://mrl.zhongyouzk.top

================================================================================
来源：http://cve.yangfankeji.com

H. 异常与错误处理
来源：http://dte.zhongyouzk.top

================================================================================
来源：http://xcj.aizwys.cn

[H01] try / catch 基础
来源：http://kto.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://myp.jinghuilouyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ljj.snrcjt.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pgu.316326.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://orr.ydzc1.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ius.dianchejie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qsa.aibaodan.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zbi.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mrp.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://vll.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://hny.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://win.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xqd.daxiang520.top

TS:   try { f(); } finally { cleanup(); }
来源：http://peo.ydzc1.top

Java: try { f(); } finally { cleanup(); }
来源：http://xji.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://puz.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xlk.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qip.cucudq.cn

[H03] 主动抛出异常
来源：http://yfi.ybcxt.top

Py:   raise ValueError("错误信息")
来源：http://swc.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kdf.havefunace.top

JS:   throw new Error("错误信息");
来源：http://nvz.fehbvm.com

TS:   throw new Error("错误信息");
来源：http://jxu.jlsjyb.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qap.haohaochexian.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wtn.hcnkem.com

Ruby: raise ArgumentError, "错误信息"
来源：http://itj.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://juw.nanxuanxn.top

[H04] 自定义异常类型
来源：http://dme.hcnkem.com

Py:   class MyError(Exception): pass
来源：http://ypk.jyoumei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rfg.zycfv.cn

JS:   class MyError extends Error {}
来源：http://xxm.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://ysq.guowangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://pse.yvedp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vfy.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://zuj.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://whr.tanke756.top

[H05] 捕获特定类型
来源：http://ovp.yuxming.cn

Py:   except ValueError as e:
来源：http://oop.yj20258888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pol.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://lvl.cucudq.cn

TS:   if (e instanceof TypeError) {}
来源：http://uzb.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://wnm.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fei.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://sen.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kqz.ybcxt.top

[H06] 可选值 / 空值安全访问
来源：http://wea.hnqzz.top

Py:   value = d.get("k") or default
来源：http://xmr.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://btx.xuanzx.com

JS:   obj?.a?.b;  d ?? default
来源：http://iuf.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://weh.tanke756.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wei.xziqi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gun.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://cgn.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://mvu.xuetiantiany.cn

[H07] 断言
来源：http://bmv.sufxvd.cn

Py:   assert x > 0, "必须为正"
来源：http://gen.shzxlz.cn

PHP:  assert($x > 0);
来源：http://rcu.yongpay.top

JS:   console.assert(x > 0);
来源：http://rqw.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://okk.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://tcl.epnwcf.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bwu.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://prc.cashguo.top

C#:   Debug.Assert(x > 0);
来源：http://xnk.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://ull.hesvh.cn

Py:   str(e);  traceback.format_exc()
来源：http://kzs.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ylc.tianlin.xyz

JS:   e.message;  e.stack
来源：http://vbh.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://xos.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pmq.jianghu66.top

Go:   err.Error()
来源：http://hae.ywan-chungtsiang.top

Ruby: e.message;  e.backtrace
来源：http://afk.yongpay.top

C#:   e.Message;  e.StackTrace
来源：http://mic.zhongyouzk.top

[H09] 带错误码的异常
来源：http://mip.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zzp.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kzv.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gpr.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yxy.kuanghao11.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://niv.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vqw.zhoulong.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ucb.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yez.zhaomingkeji.xyz

[H10] 资源自动释放
来源：http://oab.pycfn.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://mab.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://txr.nwbrower.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ayx.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sgo.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wfd.vqdsnc.cn

Go:   defer f.Close()
来源：http://iiy.gogol.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://por.yj202588.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://man.yj20258888.top

================================================================================
来源：http://pqe.aibaodan.cn

I. 正则表达式
来源：http://fdl.hysaishi.cn

================================================================================
来源：http://wcl.9152youxi.cn

[I01] 判断是否匹配
来源：http://hhx.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xrx.jlsjyb.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gkt.zhengqikj.top

JS:   /\d+/.test(s)
来源：http://xzj.guannengcc.top

TS:   /\d+/.test(s)
来源：http://ndi.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vgb.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rgs.fengsongda.top

Ruby: s.match?(/\d+/)
来源：http://oze.fktsv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nlf.ppjwa.cn

[I02] 提取所有匹配
来源：http://bhw.jinyuanbaomall.cn

Py:   re.findall(r"\d+", s)
来源：http://ekt.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bmm.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vsu.ivvv.top

TS:   s.match(/\d+/g)
来源：http://gvw.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hjt.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mcf.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://tok.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hjz.zycfv.cn

[I03] 提取捕获分组
来源：http://cwq.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lma.quarkkingdee.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hwb.nwbrower.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xau.tian-w.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ubq.epnwcf.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mze.yj202588.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hwh.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zwt.dianchejie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mep.gzhubu.top

[I04] 正则替换
来源：http://irg.gotoacloud.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fss.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ybd.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pyf.ehwqpu.com

TS:   s.replace(/\d+/g, "#")
来源：http://ioj.aizwys.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vmr.jlsjyb.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qas.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hkl.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oys.sufxvd.cn

[I05] 按正则拆分
来源：http://qrx.andypj.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://itl.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iob.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://yef.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://tkz.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://lfy.cucudq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xep.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://dvu.zdqjudy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://grp.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tlk.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yqt.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qbp.shanyushiyangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nxn.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bce.ehwqpu.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://toa.zhixingplan.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pso.nwbrower.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wdf.0kj1m.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sxv.bjfxy.top

[I07] 忽略大小写与多行模式
来源：http://kci.hysaishi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iuw.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eqr.cashguo.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eup.vehdjk.com

TS:   /error/gim
来源：http://mwl.shanyushiyangtech.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lwi.zhixingplan.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wtw.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://hub.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ciy.fehbvm.com

[I08] 贪婪与非贪婪匹配
来源：http://qvw.zdqjudy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zpw.daria6918.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sfr.xylfe.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fgq.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pua.yueranfly.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zaw.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mdo.birdmap.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bbd.hammf.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rsr.tianlin.xyz

================================================================================
来源：http://qpo.jinqigufen.top

J. 日期与时间
来源：http://eft.quarkkingdee.top

================================================================================
来源：http://kdu.yj202588.top

[J01] 获取当前时间
来源：http://kwc.yanxiufei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dgm.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nad.kuanghao11.cn

JS:   new Date();  Date.now()
来源：http://muw.nwbrower.top

TS:   new Date();  Date.now()
来源：http://ixn.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jog.uphjek.com

Go:   time.Now()
来源：http://fbx.zhiwuduotai.top

Ruby: Time.now
来源：http://env.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qkk.cdnleiting.top

[J02] 格式化输出
来源：http://gfo.fengsongda.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cmh.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sna.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qzc.gogol.net.cn

TS:   d.toISOString()
来源：http://zsl.hfpthk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xjn.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://out.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xjx.yuxming.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ume.sjlbkw.cn

[J03] 字符串解析为日期
来源：http://fra.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kox.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xey.vehdjk.com

JS:   new Date("2024-01-02")
来源：http://qwd.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://hip.sysykeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://uvj.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gxx.cqqwz.cn

Ruby: Date.parse("2024-01-02")
来源：http://tlq.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zem.andypj.xyz

[J04] 时间戳与日期互转
来源：http://tur.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kiy.chenzaomai.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vao.chenlongwang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tzi.bjfxy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://afx.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yta.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tgb.tianlin.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://act.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tgm.hcnkem.com

[J05] 时间加减（加 7 天）
来源：http://qbx.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://shy.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gsr.sweek.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yrm.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://miu.dashuyun.cn

Java: LocalDate.now().plusDays(7)
来源：http://idy.chenjidiqi.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gbe.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://jhl.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://cxk.daria6918.cn

[J06] 计算两时间之差
来源：http://tap.pycfn.com

Py:   (end - start).total_seconds()
来源：http://dwv.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://qpp.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uag.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ptx.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://muz.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://mkg.gzhubu.top

Ruby: end - start                 # 返回秒数
来源：http://oxq.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://dri.yj20258.top

[J07] 比较两个日期
来源：http://rvq.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://vlq.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dfr.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tiu.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://mke.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tnb.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ncs.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://ucf.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://pyx.yanxiufei.cn

[J08] 提取年月日与星期
来源：http://gpa.tian-w.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pvy.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lbv.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pwl.bjfxy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bde.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://beh.nanxinkj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kam.nanxuanxn.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zqc.epnwcf.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jun.hnqzz.top

[J09] 时区处理
来源：http://wgx.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ist.shanyushiyangtech.top


<!-- 参考信息 -->