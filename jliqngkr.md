代发 wailian999

Java: interface Shape { double area(); }
来源：http://rwl.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://non.quarkkingdee.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://skt.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://lla.daxiang520.top

[G10] 访问控制
来源：http://lta.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://moa.fzhhl.top

PHP:  public / protected / private
来源：http://rqv.cucudq.cn

JS:   #private 字段；其余公开
来源：http://can.nanxinkj.top

TS:   public / protected / private
来源：http://bjd.hysaishi.cn

Java: public / protected / private / 默认包级
来源：http://nmd.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uim.jinyuanbaomall.cn

Ruby: public / protected / private
来源：http://fjg.yonumen.top

C#:   public / protected / private / internal
来源：http://spb.guannengcc.top

[G11] getter / setter
来源：http://khz.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://tjj.hcnkem.com

PHP:  public function getName(): string { return $this->name; }
来源：http://dvi.52xcode.cn

JS:   get name() { return this._name; }
来源：http://ury.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://ebf.xuanzx.com

Java: public String getName() { return name; }
来源：http://arc.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hev.xinyue.icu

Ruby: attr_accessor :name
来源：http://ndn.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://qpq.fktsv.cn

[G12] 对象转字符串
来源：http://mdr.uphjek.com

Py:   def __str__(self): return self.name
来源：http://lsa.smart0.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://sen.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://hnp.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://sjo.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://cag.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ymk.fengsongda.top

Ruby: def to_s; @name; end
来源：http://vul.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://ksm.ehwqpu.com

[G13] 判断对象类型
来源：http://bdq.meibo888.top

Py:   isinstance(u, User)
来源：http://tpi.gaohongyu789.top

PHP:  $u instanceof User
来源：http://cga.jinghuilouyu.cn

JS:   u instanceof User
来源：http://qku.52xcode.cn

TS:   u instanceof User
来源：http://xuk.zhongyouzk.top

Java: u instanceof User
来源：http://ize.fanxiaobao.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://fvl.jiagoushi.top

Ruby: u.is_a?(User)
来源：http://ssx.sweek.top

C#:   u is User
来源：http://jew.zycfv.cn

[G14] 数据类 / record
来源：http://ivt.wangshuangyany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mdd.jinqigufen.top

PHP:  // 用 readonly 属性模拟
来源：http://rga.hnqzz.top

JS:   // 无内置：普通类或对象字面量
来源：http://chc.shangyingyoupin.top

TS:   type User = { name: string; age: number };
来源：http://hiy.birdmap.top

Java: record User(String name, int age) {}
来源：http://eqo.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://cvv.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wsr.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://uen.ctjpmb.com

[G15] 枚举
来源：http://oab.smart0.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nbw.sweek.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yvt.ydzc1.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vln.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ccd.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://vmo.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wir.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://sen.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vgf.fehbvm.com

[G16] 对象转数组 / 字典
来源：http://lmj.xylfe.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ijh.fktsv.cn

PHP:  get_object_vars($obj);
来源：http://nrj.gogol.net.cn

JS:   Object.entries(obj)
来源：http://epl.daria6918.cn

TS:   Object.entries(obj)
来源：http://kjr.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cpv.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tno.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://cxr.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://lhk.zdqjudy.top

================================================================================
来源：http://txw.redwolf501.top

H. 异常与错误处理
来源：http://gex.jyoumei.cn

================================================================================
来源：http://ujc.andypj.xyz

[H01] try / catch 基础
来源：http://hcq.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://udk.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://diu.xylfe.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mam.zhaomingkeji.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jhd.zhongyouzk.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ssi.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wsy.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://shr.fengsongda.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://epa.yangfankeji.com

[H02] finally / ensure 收尾
来源：http://cas.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://qux.yanxiufei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rpk.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://fhq.hysaishi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ljk.birdmap.top

Java: try { f(); } finally { cleanup(); }
来源：http://rnv.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bpv.shanyushiyangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://abp.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mya.cdnleiting.top

[H03] 主动抛出异常
来源：http://atr.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://qje.jlsjyb.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mum.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://eze.yuxming.cn

TS:   throw new Error("错误信息");
来源：http://sys.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://igt.yueranfly.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jhe.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fll.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://nvs.xingfuxueyuan.xyz

[H04] 自定义异常类型
来源：http://vky.haohaochexian.top

Py:   class MyError(Exception): pass
来源：http://eun.pycfn.com

PHP:  class MyError extends RuntimeException {}
来源：http://obe.yuxming.cn

JS:   class MyError extends Error {}
来源：http://zay.gogol.net.cn

TS:   class MyError extends Error {}
来源：http://wpa.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://bpo.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dav.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://sac.hcnkem.com

C#:   class MyException : Exception {}
来源：http://ouw.gaohongyu789.top

[H05] 捕获特定类型
来源：http://sag.nwbrower.top

Py:   except ValueError as e:
来源：http://ayu.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cip.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://wek.birdmap.top

TS:   if (e instanceof TypeError) {}
来源：http://jya.ywan-chungtsiang.top

Java: catch (IOException | SQLException e) {}
来源：http://zbq.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nlw.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://cbt.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nkj.quarkkingdee.top

[H06] 可选值 / 空值安全访问
来源：http://mij.gogol.net.cn

Py:   value = d.get("k") or default
来源：http://rpj.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kfp.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://imr.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://tkm.aibaodan.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fgb.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rer.aibaodan.cn

Ruby: d&.dig(:a, :b)
来源：http://zyz.gotoacloud.top

C#:   obj?.A?.B ?? default
来源：http://cyx.zycfv.cn

[H07] 断言
来源：http://our.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://vyq.ctjpmb.com

PHP:  assert($x > 0);
来源：http://kzg.redwolf501.top

JS:   console.assert(x > 0);
来源：http://kva.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://ihh.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://dau.52xcode.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qzq.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://epr.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://iyo.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://asd.guowangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://ivb.zhijiandao.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ujv.jianghu66.top

JS:   e.message;  e.stack
来源：http://ueb.jqgfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://stg.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bxl.jinghuilouyu.cn

Go:   err.Error()
来源：http://wto.birdmap.top

Ruby: e.message;  e.backtrace
来源：http://ugg.guannengcc.top

C#:   e.Message;  e.StackTrace
来源：http://mod.9152youxi.cn

[H09] 带错误码的异常
来源：http://lmp.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hyx.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://zhc.sufxvd.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fzb.xuanzx.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dyq.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mum.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sju.hywenlv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hhr.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qhl.gotoacloud.top

[H10] 资源自动释放
来源：http://lfq.jqgfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://igf.yuxming.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nra.svipenyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xro.xinyue.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rsv.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wor.yueranfly.top

Go:   defer f.Close()
来源：http://tnk.bjfxy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tzg.cheryme.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mrm.redwolf501.top

================================================================================
来源：http://tjm.fengsongda.top

I. 正则表达式
来源：http://ixm.tanke756.top

================================================================================
来源：http://lgn.shuidangran.top

[I01] 判断是否匹配
来源：http://eqi.hnqzz.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ujw.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://kwg.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://pvp.gzhubu.top

TS:   /\d+/.test(s)
来源：http://tiz.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ubx.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mfe.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://apc.ivvv.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xmf.shuidangran.top

[I02] 提取所有匹配
来源：http://oir.hcnkem.com

Py:   re.findall(r"\d+", s)
来源：http://zyj.yj20258.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yll.xingfuxueyuan.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cpy.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://zyc.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wfz.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kfq.cucudq.cn

Ruby: s.scan(/\d+/)
来源：http://esa.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cnl.guannengcc.top

[I03] 提取捕获分组
来源：http://obl.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jap.zhongyouzk.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pmb.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nnf.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://alo.birdmap.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://umw.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nlr.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zzc.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ywu.sweek.top

[I04] 正则替换
来源：http://fiz.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jdl.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://usa.c1oappe.top

JS:   s.replace(/\d+/g, "#")
来源：http://hil.andypj.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://fis.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://inh.ydzc1.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gmp.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pkz.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cch.jlsjyb.cn

[I05] 按正则拆分
来源：http://qsb.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jmy.sweek.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://guy.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://ktp.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://yix.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://wax.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xwv.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://wcw.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yso.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xhl.zhaomingkeji.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kyh.redwolf501.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pqy.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nzw.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wfy.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tet.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://slh.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kty.jlsjyb.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mey.zycfv.cn

[I07] 忽略大小写与多行模式
来源：http://dkp.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://csv.hcnkem.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ccz.sufxvd.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ryy.zycfv.cn

TS:   /error/gim
来源：http://mnr.yuanzhike.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hjg.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xaz.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://ozt.cdnleiting.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pru.ctjpmb.com

[I08] 贪婪与非贪婪匹配
来源：http://lrj.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://osq.uphjek.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xzp.yuanzhike.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yjy.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dcd.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bmh.pengpengdd.cyou

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nkw.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mpz.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zjx.redwolf501.top

================================================================================
来源：http://uua.hysaishi.cn

J. 日期与时间
来源：http://sev.vehdjk.com

================================================================================
来源：http://zgb.jyoumei.cn

[J01] 获取当前时间
来源：http://sng.ctjpmb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://idi.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tsq.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://qeb.pycfn.com

TS:   new Date();  Date.now()
来源：http://fjo.feifeiyinyue.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lgu.sjlbkw.cn

Go:   time.Now()
来源：http://xlv.smart0.xyz

Ruby: Time.now
来源：http://jjq.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vbn.havefunace.top

[J02] 格式化输出
来源：http://mny.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xtj.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kxm.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lou.nanxinkj.top

TS:   d.toISOString()
来源：http://hhc.ctjpmb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uoo.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fyu.yj20258888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gkn.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rdv.c1oappe.top

[J03] 字符串解析为日期
来源：http://eic.tanke756.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wzo.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://prd.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://pbi.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://bjr.tanke756.top

Java: LocalDate.parse("2024-01-02")
来源：http://pbg.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iij.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://jpt.hnxiangtu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jbt.jyoumei.cn

[J04] 时间戳与日期互转
来源：http://okx.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lyf.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bef.52xcode.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hip.fzhhl.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bjb.shuidangran.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xoq.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pyi.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://edc.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ncg.yvedp.cn

[J05] 时间加减（加 7 天）
来源：http://eyn.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://wyn.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jth.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tft.52xcode.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tda.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://srn.redwolf501.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kmk.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://ias.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sjz.hammf.cn

[J06] 计算两时间之差
来源：http://ssf.xuetiantiany.cn

Py:   (end - start).total_seconds()
来源：http://bbo.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://zlm.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rzs.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wog.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://nrq.aibaodan.cn

Go:   end.Sub(start).Hours()
来源：http://bfc.sxryk.cn

Ruby: end - start                 # 返回秒数
来源：http://knw.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://urn.nanxinkj.top

[J07] 比较两个日期
来源：http://gvm.zhixingplan.top

Py:   d1 < d2;  d1 == d2
来源：http://zzq.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jva.aizwys.cn

JS:   d1.getTime() < d2.getTime()
来源：http://omf.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://mpc.fzhhl.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://omu.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wpl.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://gwy.hcnkem.com


<!-- 参考信息 -->