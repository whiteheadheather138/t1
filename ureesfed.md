代发 wailian999

C#:   public / protected / private / internal
来源：http://dzs.yj20258888.top

[G11] getter / setter
来源：http://uhd.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://bnq.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lcf.xuanzx.com

JS:   get name() { return this._name; }
来源：http://icy.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://bgn.bbcook.cn

Java: public String getName() { return name; }
来源：http://lfg.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gta.nwbrower.top

Ruby: attr_accessor :name
来源：http://emi.yj20258.top

C#:   public string Name { get; set; }
来源：http://zqd.zhijiandao.cn

[G12] 对象转字符串
来源：http://sen.iojbl.cn

Py:   def __str__(self): return self.name
来源：http://aqt.snrcjt.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ovr.yvedp.cn

JS:   toString() { return this.name; }
来源：http://tzm.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://cgx.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://oki.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xeb.haohaochexian.top

Ruby: def to_s; @name; end
来源：http://epv.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://rrb.dashuyun.cn

[G13] 判断对象类型
来源：http://oib.hfpthk.cn

Py:   isinstance(u, User)
来源：http://idw.zhixingplan.top

PHP:  $u instanceof User
来源：http://edh.fzhhl.top

JS:   u instanceof User
来源：http://vhk.pycfn.com

TS:   u instanceof User
来源：http://ajs.zhoulong.xyz

Java: u instanceof User
来源：http://jqm.52xcode.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wcb.tarul.cn

Ruby: u.is_a?(User)
来源：http://zik.hnqzz.top

C#:   u is User
来源：http://ngc.xinyue.icu

[G14] 数据类 / record
来源：http://pjy.jinqigfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jew.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://arj.316326.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://jrb.uphjek.com

TS:   type User = { name: string; age: number };
来源：http://los.xziqi.cn

Java: record User(String name, int age) {}
来源：http://sbb.yuanzhike.top

Go:   type User struct { Name string; Age int }
来源：http://pmj.gogol.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jku.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://xps.zycfv.cn

[G15] 枚举
来源：http://qwf.cdnleiting.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zzt.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://oiw.zhixingplan.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bao.daxiang520.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wsr.jianghu66.top

Java: enum Color { RED, GREEN }
来源：http://gzr.yuxming.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sxv.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://hub.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kbv.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://jiy.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xny.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://jmm.xylfe.cn

JS:   Object.entries(obj)
来源：http://obv.epnwcf.com

TS:   Object.entries(obj)
来源：http://rpo.andypj.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gtn.havefunace.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dru.hcnkem.com

Ruby: obj.instance_variables
来源：http://jko.mhx1999.top

C#:   // 用反射或 System.Text.Json
来源：http://mhk.cashguo.top

================================================================================
来源：http://gmc.hammf.cn

H. 异常与错误处理
来源：http://rnm.ctjpmb.com

================================================================================
来源：http://dqj.wangdashe.top

[H01] try / catch 基础
来源：http://qvz.chenjidiqi.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gqr.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vou.yuxming.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ebm.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://amn.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dee.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://frz.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gqv.xylfe.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hnm.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://glf.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://ytb.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://phl.sxryk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://szo.hnxiangtu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qtp.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://axo.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ily.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://nzb.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yzn.yj20258888.top

[H03] 主动抛出异常
来源：http://sjw.zdbjq.cn

Py:   raise ValueError("错误信息")
来源：http://xjc.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zci.xinyue.icu

JS:   throw new Error("错误信息");
来源：http://jnp.redwolf501.top

TS:   throw new Error("错误信息");
来源：http://zfg.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://enk.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dkx.jqgufenzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://onc.zhongyouzk.top

C#:   throw new ArgumentException("错误信息");
来源：http://bqw.wangdashe.top

[H04] 自定义异常类型
来源：http://sib.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://qlg.guannengcc.top

PHP:  class MyError extends RuntimeException {}
来源：http://gmt.zhaomingkeji.xyz

JS:   class MyError extends Error {}
来源：http://ams.jinqigufen.top

TS:   class MyError extends Error {}
来源：http://sze.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://tet.svipenyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://onf.tianlin.xyz

Ruby: class MyError < StandardError; end
来源：http://mbc.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://lxy.yongpay.top

[H05] 捕获特定类型
来源：http://ing.shzxlz.cn

Py:   except ValueError as e:
来源：http://xyg.gaohongyu789.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://axf.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://cur.svipenyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://ogw.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://cgb.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qaw.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://xon.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wkr.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://xxd.jinqigfzy.top

Py:   value = d.get("k") or default
来源：http://wsq.ybcxt.top

PHP:  $v = $d["k"] ?? null;
来源：http://ytj.zdbjq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bbg.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://cwj.jqgfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bue.andypj.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://cve.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://xlv.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://ctk.zdbjq.cn

[H07] 断言
来源：http://cfq.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://gbw.yj20258888.top

PHP:  assert($x > 0);
来源：http://ymx.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://kud.mhx1999.top

TS:   console.assert(x > 0);
来源：http://dbs.haohaochexian.top

Java: assert x > 0 : "必须为正";
来源：http://elm.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://odq.mhx1999.top

Ruby: raise "必须为正" unless x > 0
来源：http://wok.sysykeji.top

C#:   Debug.Assert(x > 0);
来源：http://hfw.ybcxt.top

[H08] 获取错误信息与堆栈
来源：http://qan.fanxiaobao.xyz

Py:   str(e);  traceback.format_exc()
来源：http://dth.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nvb.tarul.cn

JS:   e.message;  e.stack
来源：http://zkz.cucudq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wmy.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dfh.zhiwuduotai.top

Go:   err.Error()
来源：http://nff.hfpthk.cn

Ruby: e.message;  e.backtrace
来源：http://mpv.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://zku.c1oappe.top

[H09] 带错误码的异常
来源：http://jgq.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qvy.jqgfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lrj.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hae.jlsjyb.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blo.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jwm.yfazqb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aen.svipenyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uwm.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://brc.zhoulong.xyz

[H10] 资源自动释放
来源：http://rta.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bnp.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mdx.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gdr.quarkkingdee.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xrz.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zei.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://vol.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mzw.feifeiyinyue.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zah.ywan-chungtsiang.top

================================================================================
来源：http://owl.cqqwz.cn

I. 正则表达式
来源：http://wwh.9152youxi.cn

================================================================================
来源：http://ezd.epnwcf.com

[I01] 判断是否匹配
来源：http://lia.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://egt.xingfuxueyuan.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://cfp.svipenyu.cn

JS:   /\d+/.test(s)
来源：http://ygm.hnqzz.top

TS:   /\d+/.test(s)
来源：http://rcb.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hyw.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dka.ctjpmb.com

Ruby: s.match?(/\d+/)
来源：http://okq.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wbi.jqgufenzy.top

[I02] 提取所有匹配
来源：http://wns.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://pqb.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mni.yuanzhike.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://txn.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://lwp.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ygi.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jdp.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://jvb.yj202588.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ovj.yj20258.top

[I03] 提取捕获分组
来源：http://att.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lsx.daria6918.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qra.xinyue.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rsb.fzhhl.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sgr.birdmap.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vjc.shanyushiyangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://awc.ydjk.org.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lzb.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sbk.wangdashe.top

[I04] 正则替换
来源：http://zrv.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qfl.snrcjt.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yso.cqqwz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://blb.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gkj.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://xnq.sjlbkw.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ccq.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wur.jqgufenzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ais.fzhhl.top

[I05] 按正则拆分
来源：http://xln.ivvv.top

Py:   re.split(r"\s*,\s*", s)
来源：http://izc.pengpengdd.cyou

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mmw.yuxming.cn

JS:   s.split(/\s*,\s*/)
来源：http://jlu.meibo888.top

TS:   s.split(/\s*,\s*/)
来源：http://rvp.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://fvo.daria6918.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ysc.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ijt.wangdashe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://scp.jyoumei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://glk.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zbp.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gpv.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://chg.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bic.jinqigufen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lvz.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://upk.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://inp.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zty.jinyuanbaomall.cn

[I07] 忽略大小写与多行模式
来源：http://nmt.cucudq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xoi.tanke756.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hrb.quarkkingdee.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pco.hnxiangtu.top

TS:   /error/gim
来源：http://rxb.c1oappe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pcs.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mpe.svipenyu.cn

Ruby: s.scan(/error/i)
来源：http://sxx.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tda.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://uoq.zhongyouzk.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gam.ivvv.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yud.shanyushiyangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fhb.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yim.zhiwuduotai.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ate.sysykeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mlk.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eqw.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zvm.zhixingplan.top

================================================================================
来源：http://ufr.tanke756.top

J. 日期与时间
来源：http://sjv.jianghu66.top

================================================================================
来源：http://klk.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://zuh.yonumen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bme.jinyuanbaomall.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nal.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://ghn.havefunace.top

TS:   new Date();  Date.now()
来源：http://muw.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hgk.hesvh.cn

Go:   time.Now()
来源：http://rpp.bjfxy.top

Ruby: Time.now
来源：http://atq.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://umo.wangshuangyany.cn

[J02] 格式化输出
来源：http://acr.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ekk.fzhhl.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fqk.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jpc.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://gew.tarul.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nly.hfpthk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cgv.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uoy.jinyuanbaomall.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uca.smart0.xyz

[J03] 字符串解析为日期
来源：http://gxv.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bsj.sweek.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fms.yuanzhike.top

JS:   new Date("2024-01-02")
来源：http://utd.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://xbc.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ufk.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tcf.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://rwi.ehwqpu.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qre.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://ihg.fanxiaobao.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cub.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vem.52xcode.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qwz.yfazqb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://ame.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://agk.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gih.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qox.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eqg.fzhhl.top

[J05] 时间加减（加 7 天）
来源：http://jkk.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://cef.9152youxi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://snh.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pkh.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wtk.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://fgg.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://put.gzhubu.top

Ruby: Time.now + 7 * 86400
来源：http://kbt.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://qkq.chenlongwang.top

[J06] 计算两时间之差
来源：http://geq.meibo888.top

Py:   (end - start).total_seconds()
来源：http://yvf.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://ftd.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sok.xuanzx.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ida.hysaishi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gjc.bbcook.cn

Go:   end.Sub(start).Hours()
来源：http://gct.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://pif.zhaomingkeji.xyz

C#:   (end - start).TotalSeconds
来源：http://dcc.birdmap.top

[J07] 比较两个日期
来源：http://ybr.zhixingplan.top

Py:   d1 < d2;  d1 == d2
来源：http://mkp.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iko.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gmn.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://bpb.fehbvm.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bxp.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tgt.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://jxs.shangyingyoupin.top

C#:   d1 < d2;  d1 == d2
来源：http://dij.9152youxi.cn

[J08] 提取年月日与星期
来源：http://wlu.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xuy.bjfxy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://djj.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hzk.cqqwz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oun.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jwk.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bzf.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tdu.hongshengwenyu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nnn.0kj1m.cn

[J09] 时区处理
来源：http://hrt.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bnw.ivvv.top


<!-- 参考信息 -->