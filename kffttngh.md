代发 wailian999

TS:   public / protected / private
来源：http://cis.havefunace.top

Java: public / protected / private / 默认包级
来源：http://hki.mhx1999.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ihg.hysaishi.cn

Ruby: public / protected / private
来源：http://bey.aibaodan.cn

C#:   public / protected / private / internal
来源：http://ckt.yj20258888.top

[G11] getter / setter
来源：http://vhr.pycfn.com

Py:   @property 与 @x.setter
来源：http://eit.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jrw.fehbvm.com

JS:   get name() { return this._name; }
来源：http://pep.sweek.top

TS:   get name(): string { return this._name; }
来源：http://jha.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://pss.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://xan.cdnleiting.top

Ruby: attr_accessor :name
来源：http://cfm.sysykeji.top

C#:   public string Name { get; set; }
来源：http://prj.yj20258.top

[G12] 对象转字符串
来源：http://bph.jinyuanbaomall.cn

Py:   def __str__(self): return self.name
来源：http://yix.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://ebz.xylfe.cn

JS:   toString() { return this.name; }
来源：http://kjd.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://sbq.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://xdw.yfazqb.com

Go:   func (u User) String() string { return u.Name }
来源：http://xlj.gaohongyu789.top

Ruby: def to_s; @name; end
来源：http://iiz.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://bqx.yangfankeji.com

[G13] 判断对象类型
来源：http://tgq.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://jvu.jyoumei.cn

PHP:  $u instanceof User
来源：http://mzi.svipenyu.cn

JS:   u instanceof User
来源：http://wat.fktsv.cn

TS:   u instanceof User
来源：http://art.c1oappe.top

Java: u instanceof User
来源：http://xmu.aizwys.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tbv.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://uel.ydjk.org.cn

C#:   u is User
来源：http://ual.kuanghao11.cn

[G14] 数据类 / record
来源：http://unq.yanxiufei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wnj.yj202588.top

PHP:  // 用 readonly 属性模拟
来源：http://cgv.zhaomingkeji.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://jnc.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://ohz.redwolf501.top

Java: record User(String name, int age) {}
来源：http://zbc.yuxming.cn

Go:   type User struct { Name string; Age int }
来源：http://hns.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://snh.ctjpmb.com

C#:   record User(string Name, int Age);
来源：http://bom.sweek.top

[G15] 枚举
来源：http://cdy.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mkh.uphjek.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://bhr.yongpay.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kqe.fanxiaobao.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cji.quarkkingdee.top

Java: enum Color { RED, GREEN }
来源：http://poq.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lfk.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://lgf.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mvu.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://hli.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hsv.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://wsl.fktsv.cn

JS:   Object.entries(obj)
来源：http://mox.hammf.cn

TS:   Object.entries(obj)
来源：http://rmo.jyoumei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nrj.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://twi.snrcjt.cn

Ruby: obj.instance_variables
来源：http://war.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://abq.cdnleiting.top

================================================================================
来源：http://saj.pycfn.com

H. 异常与错误处理
来源：http://evr.shuidangran.top

================================================================================
来源：http://yhw.tian-w.cn

[H01] try / catch 基础
来源：http://evz.wangdashe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mcw.gzhubu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ufj.xziqi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wjp.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://esx.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yod.fanxiaobao.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mff.xylfe.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pyy.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sku.daxiang520.top

[H02] finally / ensure 收尾
来源：http://bge.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://ozq.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ums.hysaishi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://eji.yongpay.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nos.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://vra.gogol.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cdw.andypj.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://skd.cqqwz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jzq.sjlbkw.cn

[H03] 主动抛出异常
来源：http://lof.tanke756.top

Py:   raise ValueError("错误信息")
来源：http://brz.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://phx.haohaochexian.top

JS:   throw new Error("错误信息");
来源：http://olh.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://byv.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lfc.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ebv.hysaishi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ktg.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://erc.sxryk.cn

[H04] 自定义异常类型
来源：http://ikc.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://emi.shuidangran.top

PHP:  class MyError extends RuntimeException {}
来源：http://ksj.yongpay.top

JS:   class MyError extends Error {}
来源：http://zdq.shangyingyoupin.top

TS:   class MyError extends Error {}
来源：http://eln.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://vbz.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eee.pycfn.com

Ruby: class MyError < StandardError; end
来源：http://lgx.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://roa.kuanghao11.cn

[H05] 捕获特定类型
来源：http://hha.ivvv.top

Py:   except ValueError as e:
来源：http://flo.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qdq.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://vmb.cheryme.top

TS:   if (e instanceof TypeError) {}
来源：http://ted.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://rtq.tian-w.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zvg.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://cgw.yj20258.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zyw.xuetiantiany.cn

[H06] 可选值 / 空值安全访问
来源：http://hkr.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://gqh.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mxt.yj202588.top

JS:   obj?.a?.b;  d ?? default
来源：http://zdc.bbcook.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uds.bbcook.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ulu.cdnleiting.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cev.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://kem.jianghu66.top

C#:   obj?.A?.B ?? default
来源：http://bur.52xcode.cn

[H07] 断言
来源：http://vvu.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://vqx.cucudq.cn

PHP:  assert($x > 0);
来源：http://cil.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://mxd.gogol.net.cn

TS:   console.assert(x > 0);
来源：http://owk.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://isx.redwolf501.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ttm.jinqigufen.top

Ruby: raise "必须为正" unless x > 0
来源：http://njn.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://ouf.tian-w.cn

[H08] 获取错误信息与堆栈
来源：http://seq.cashguo.top

Py:   str(e);  traceback.format_exc()
来源：http://asn.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oom.ydzc1.top

JS:   e.message;  e.stack
来源：http://cym.ydjk.org.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kop.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vro.haohaochexian.top

Go:   err.Error()
来源：http://tlr.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://lir.sjlbkw.cn

C#:   e.Message;  e.StackTrace
来源：http://uzh.52xcode.cn

[H09] 带错误码的异常
来源：http://yvy.svipenyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://icv.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://fhf.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xct.dashuyun.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mxm.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://teh.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pnk.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://uge.xziqi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rba.c1oappe.top

[H10] 资源自动释放
来源：http://jib.zdbjq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dea.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.sxryk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vcd.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mfx.xylfe.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rws.zdqjudy.top

Go:   defer f.Close()
来源：http://tao.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lkv.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ncu.nanxuanxn.top

================================================================================
来源：http://hhp.cheryme.top

I. 正则表达式
来源：http://uuc.ybcxt.top

================================================================================
来源：http://bvb.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://yly.xuanzx.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://txh.tarul.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dmt.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://cwu.ivvv.top

TS:   /\d+/.test(s)
来源：http://ayw.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://scd.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yut.wangdashe.top

Ruby: s.match?(/\d+/)
来源：http://jwt.cqqwz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mid.gogol.net.cn

[I02] 提取所有匹配
来源：http://err.gzhubu.top

Py:   re.findall(r"\d+", s)
来源：http://hsc.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hzq.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oqc.sjlbkw.cn

TS:   s.match(/\d+/g)
来源：http://mly.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pxq.yfazqb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://giw.hysaishi.cn

Ruby: s.scan(/\d+/)
来源：http://iuh.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mte.tian-w.cn

[I03] 提取捕获分组
来源：http://abo.yuxming.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sdl.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://llm.xuetiantiany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jqr.gaohongyu789.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qen.xziqi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pdx.shanyushiyangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://acj.xuanzx.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ezp.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uqm.zhiwuduotai.top

[I04] 正则替换
来源：http://man.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jur.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hhx.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://wuk.zdqjudy.top

TS:   s.replace(/\d+/g, "#")
来源：http://ejs.nwbrower.top

Java: s.replaceAll("\\d+", "#")
来源：http://vwh.shanyushiyangtech.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hrc.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://bgw.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xkh.zdqjudy.top

[I05] 按正则拆分
来源：http://uzf.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://ubv.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://htd.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://oqz.havefunace.top

TS:   s.split(/\s*,\s*/)
来源：http://dtm.meibo888.top

Java: s.split("\\s*,\\s*")
来源：http://stb.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qsl.pengpengdd.cyou

Ruby: s.split(/\s*,\s*/)
来源：http://jvc.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://okn.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ogp.aibaodan.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kan.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://smr.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cpj.zhongyouzk.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fth.jlsjyb.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rho.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://edb.jinyuanbaomall.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zpx.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rhq.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://wku.jyoumei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hjn.xuetiantiany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wjm.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ccm.jyoumei.cn

TS:   /error/gim
来源：http://xaz.hfpthk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aro.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hlj.haohaochexian.top

Ruby: s.scan(/error/i)
来源：http://sjt.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nvf.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://xyd.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sfw.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ukh.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xzq.hfpthk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jhu.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uho.fehbvm.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jhe.sufxvd.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lmc.pycfn.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bcw.ydjk.org.cn

================================================================================
来源：http://ere.yonumen.top

J. 日期与时间
来源：http://ybf.dianchejie.cn

================================================================================
来源：http://ghc.haohaochexian.top

[J01] 获取当前时间
来源：http://dfz.shzxlz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cvz.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xro.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://pkp.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://hlm.tian-w.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hdq.tian-w.cn

Go:   time.Now()
来源：http://gdg.dashuyun.cn

Ruby: Time.now
来源：http://ukk.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lkt.hnqzz.top

[J02] 格式化输出
来源：http://mao.hnxiangtu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ubx.fktsv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xvb.yvedp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rjv.yongpay.top

TS:   d.toISOString()
来源：http://dgt.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://opf.hnqzz.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iiz.uphjek.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cpa.hammf.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vzv.chenjidiqi.icu

[J03] 字符串解析为日期
来源：http://eum.smart0.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ubi.cheryme.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gfh.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://grr.xuanzx.com

TS:   new Date("2024-01-02")
来源：http://wkw.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://vmk.uphjek.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vhn.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://uya.hfpthk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://luy.hywenlv.cn

[J04] 时间戳与日期互转
来源：http://auq.wangdashe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cti.zdbjq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vfw.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ssg.ybcxt.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jvq.redwolf501.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xmt.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zge.xuetiantiany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pjd.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qdi.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://swc.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://kan.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cef.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ott.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gdx.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://jdz.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hap.52xcode.cn

Ruby: Time.now + 7 * 86400
来源：http://oxi.guowangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://bdp.jlsjyb.cn

[J06] 计算两时间之差
来源：http://uxb.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://ten.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://gzq.tian-w.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://klb.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tmo.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://pnk.fanxiaobao.xyz

Go:   end.Sub(start).Hours()
来源：http://wfc.nanxuanxn.top

Ruby: end - start                 # 返回秒数
来源：http://meh.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://yxd.fktsv.cn

[J07] 比较两个日期
来源：http://ffd.wangdashe.top

Py:   d1 < d2;  d1 == d2
来源：http://vxm.ppjwa.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bpe.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://dcu.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://umt.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eqi.tianlin.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jqo.chenjidiqi.icu

Ruby: d1 < d2;  d1 == d2
来源：http://fkl.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://shx.yangfankeji.com

[J08] 提取年月日与星期
来源：http://doi.fengsongda.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bti.xuanzx.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kfj.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tav.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lag.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://glr.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zne.zhongyouzk.top


<!-- 参考信息 -->