代发 wailian999

C#:   public / protected / private / internal
来源：http://ity.pycfn.com

[G11] getter / setter
来源：http://ieu.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://pmh.gaohongyu789.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fsl.xuanzx.com

JS:   get name() { return this._name; }
来源：http://rnh.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://nhc.ppjwa.cn

Java: public String getName() { return name; }
来源：http://qhh.yvedp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fjl.aizwys.cn

Ruby: attr_accessor :name
来源：http://avs.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://bba.hongshengwenyu.top

[G12] 对象转字符串
来源：http://wzc.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://uob.zhijiandao.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bmy.ppjwa.cn

JS:   toString() { return this.name; }
来源：http://aux.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://esl.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://int.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tym.sufxvd.cn

Ruby: def to_s; @name; end
来源：http://dfy.iojbl.cn

C#:   public override string ToString() => Name;
来源：http://ois.guannengcc.top

[G13] 判断对象类型
来源：http://kks.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://atg.yj202588.top

PHP:  $u instanceof User
来源：http://vwb.xylfe.cn

JS:   u instanceof User
来源：http://toe.vqdsnc.cn

TS:   u instanceof User
来源：http://qrt.gogol.net.cn

Java: u instanceof User
来源：http://pvu.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ilh.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://odz.hcnkem.com

C#:   u is User
来源：http://vtz.bjfxy.top

[G14] 数据类 / record
来源：http://vcp.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pkq.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://mfr.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://zfj.birdmap.top

TS:   type User = { name: string; age: number };
来源：http://dgm.yj20258.top

Java: record User(String name, int age) {}
来源：http://mtg.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://dob.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fbv.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://cej.yuxming.cn

[G15] 枚举
来源：http://yhy.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vvm.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ppy.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pmy.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tqe.hfpthk.cn

Java: enum Color { RED, GREEN }
来源：http://fhi.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wbw.yvedp.cn

Ruby: Color = %i[red green].freeze
来源：http://vuo.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rgk.316326.xyz

[G16] 对象转数组 / 字典
来源：http://kdd.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ltv.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://kvh.yonumen.top

JS:   Object.entries(obj)
来源：http://jdh.kuanghao11.cn

TS:   Object.entries(obj)
来源：http://xou.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vbf.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ovx.yangfankeji.com

Ruby: obj.instance_variables
来源：http://knm.sxryk.cn

C#:   // 用反射或 System.Text.Json
来源：http://rpc.tian-w.cn

================================================================================
来源：http://ikl.hnqzz.top

H. 异常与错误处理
来源：http://ilz.sysykeji.top

================================================================================
来源：http://zcj.cucudq.cn

[H01] try / catch 基础
来源：http://bpd.jianghu66.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iao.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cnk.havefunace.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ggy.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ufv.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nzu.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rsj.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cix.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kfy.shuidangran.top

[H02] finally / ensure 收尾
来源：http://buk.guannengcc.top

Py:   try: f()⏎finally: cleanup()
来源：http://thp.sysykeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gld.hywenlv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ljv.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vzx.guowangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://zhb.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://euw.zdqjudy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zsy.havefunace.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://itm.jlsjyb.cn

[H03] 主动抛出异常
来源：http://ixy.xinyue.icu

Py:   raise ValueError("错误信息")
来源：http://sxy.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dby.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://hlr.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://zmn.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xat.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ggs.xingfuxueyuan.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://szq.zhijiandao.cn

C#:   throw new ArgumentException("错误信息");
来源：http://enm.sufxvd.cn

[H04] 自定义异常类型
来源：http://bxf.fzhhl.top

Py:   class MyError(Exception): pass
来源：http://nru.nwbrower.top

PHP:  class MyError extends RuntimeException {}
来源：http://nbx.quarkkingdee.top

JS:   class MyError extends Error {}
来源：http://pda.fanxiaobao.xyz

TS:   class MyError extends Error {}
来源：http://zpm.shanyushiyangtech.top

Java: class MyException extends RuntimeException {}
来源：http://swx.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mjf.zhiwuduotai.top

Ruby: class MyError < StandardError; end
来源：http://cau.zdbjq.cn

C#:   class MyException : Exception {}
来源：http://mwa.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://dst.guowangkeji.top

Py:   except ValueError as e:
来源：http://qzw.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fpc.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://bfd.jlsjyb.cn

TS:   if (e instanceof TypeError) {}
来源：http://gua.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://qpv.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://den.wangdashe.top

Ruby: rescue ArgumentError => e
来源：http://dvy.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zfk.xingfuxueyuan.xyz

[H06] 可选值 / 空值安全访问
来源：http://afg.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://kyp.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://ctc.zdbjq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pho.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://zmu.xinyue.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xid.xuetiantiany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ken.jinqigfzy.top

Ruby: d&.dig(:a, :b)
来源：http://ron.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://zoh.hesvh.cn

[H07] 断言
来源：http://wru.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://vkc.jinghuilouyu.cn

PHP:  assert($x > 0);
来源：http://kzl.tanke756.top

JS:   console.assert(x > 0);
来源：http://lwi.shuidangran.top

TS:   console.assert(x > 0);
来源：http://qqk.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://dzp.chenjidiqi.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wcw.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://man.xziqi.cn

C#:   Debug.Assert(x > 0);
来源：http://ppl.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://lgq.zhiwuduotai.top

Py:   str(e);  traceback.format_exc()
来源：http://brz.bbcook.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://euu.shzxlz.cn

JS:   e.message;  e.stack
来源：http://lye.gzhubu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cpq.xziqi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ugo.yuxming.cn

Go:   err.Error()
来源：http://mpm.jqgfzy.top

Ruby: e.message;  e.backtrace
来源：http://zij.ydjk.org.cn

C#:   e.Message;  e.StackTrace
来源：http://sve.hysaishi.cn

[H09] 带错误码的异常
来源：http://hdk.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ctz.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://snt.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tbp.yj20258888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vxx.jinqigfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rxl.hnxiangtu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eif.zdqjudy.top

Ruby: raise MyError.new("fail", 500)
来源：http://ywt.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://wxn.yfazqb.com

[H10] 资源自动释放
来源：http://ssd.jinqigfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gjo.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nco.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pef.shangyingyoupin.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yiu.shzxlz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kbz.yj20258.top

Go:   defer f.Close()
来源：http://rtw.hongshengwenyu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mta.zhaomingkeji.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nbx.fanxiaobao.xyz

================================================================================
来源：http://krr.jqgufenzy.top

I. 正则表达式
来源：http://dbp.zdqjudy.top

================================================================================
来源：http://hxx.zhongyouzk.top

[I01] 判断是否匹配
来源：http://rim.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gwl.xingfuxueyuan.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://uyx.meibo888.top

JS:   /\d+/.test(s)
来源：http://bok.kuanghao11.cn

TS:   /\d+/.test(s)
来源：http://jld.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kjx.yfazqb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mjb.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://gxi.xylfe.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iyx.fktsv.cn

[I02] 提取所有匹配
来源：http://lsz.cqqwz.cn

Py:   re.findall(r"\d+", s)
来源：http://nxg.zhongyouzk.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mnk.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rle.cheryme.top

TS:   s.match(/\d+/g)
来源：http://zss.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eau.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cha.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://ejv.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://egs.hcnkem.com

[I03] 提取捕获分组
来源：http://lbo.birdmap.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vxy.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zjf.316326.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wiw.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lyf.zhengqikj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ftc.zhijiandao.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jlm.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://odo.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cvq.sjlbkw.cn

[I04] 正则替换
来源：http://guu.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://fls.jinqigufen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://amy.svipenyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xlm.meibo888.top

TS:   s.replace(/\d+/g, "#")
来源：http://zdu.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://dbq.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vzg.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kuo.yj20258.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://myp.sweek.top

[I05] 按正则拆分
来源：http://yzf.pengpengdd.cyou

Py:   re.split(r"\s*,\s*", s)
来源：http://xss.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gcj.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://moc.52xcode.cn

TS:   s.split(/\s*,\s*/)
来源：http://kfw.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://hhj.jyoumei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://umd.hfpthk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gdz.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lis.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://brj.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qqv.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kwq.shanyushiyangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nch.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://akc.vehdjk.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mks.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xuf.chenjidiqi.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lfh.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yho.yj202588.top

[I07] 忽略大小写与多行模式
来源：http://ujj.quarkkingdee.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oip.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wjy.sjlbkw.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ctl.shanyushiyangtech.top

TS:   /error/gim
来源：http://vft.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kdi.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hfd.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://kvh.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sea.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://fuy.daria6918.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qjh.jiagoushi.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ral.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gto.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mgv.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://uja.gotoacloud.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uea.haohaochexian.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gvj.haohaochexian.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://clr.yuanzhike.top

================================================================================
来源：http://ius.hnxiangtu.top

J. 日期与时间
来源：http://ots.hongshengwenyu.top

================================================================================
来源：http://uto.uphjek.com

[J01] 获取当前时间
来源：http://asi.epnwcf.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ujb.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://okf.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://tmd.epnwcf.com

TS:   new Date();  Date.now()
来源：http://qhi.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ciq.jiagoushi.top

Go:   time.Now()
来源：http://zeu.jinqigfzy.top

Ruby: Time.now
来源：http://oeb.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qjv.ydzc1.top

[J02] 格式化输出
来源：http://qbh.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ayx.tanke756.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://loh.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nvw.jyoumei.cn

TS:   d.toISOString()
来源：http://rfn.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rdf.yfazqb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sqs.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ckg.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mqk.hysaishi.cn

[J03] 字符串解析为日期
来源：http://oqu.yanxiufei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ioa.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://roj.bjfxy.top

JS:   new Date("2024-01-02")
来源：http://hzv.gaohongyu789.top

TS:   new Date("2024-01-02")
来源：http://vkq.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ygp.ehwqpu.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wxi.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://dgn.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vrc.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://tzb.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xds.nwbrower.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jsa.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rag.birdmap.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ufs.zdqjudy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ijn.pycfn.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bvl.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ayz.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yed.yfazqb.com

[J05] 时间加减（加 7 天）
来源：http://zyr.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://ypi.yangfankeji.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://rtk.zhijiandao.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fjy.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://app.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://iqn.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cmo.c1oappe.top

Ruby: Time.now + 7 * 86400
来源：http://vgh.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://gjh.shanyushiyangkeji.top

[J06] 计算两时间之差
来源：http://nir.cheryme.top

Py:   (end - start).total_seconds()
来源：http://iah.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://pbd.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wtf.yuanzhike.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wyv.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kce.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://hig.hcnkem.com

Ruby: end - start                 # 返回秒数
来源：http://vrg.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://mfx.sjlbkw.cn

[J07] 比较两个日期
来源：http://sty.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://fup.shuidangran.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rig.shuidangran.top

JS:   d1.getTime() < d2.getTime()
来源：http://dnr.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://jju.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jrz.fehbvm.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://okj.hnqzz.top

Ruby: d1 < d2;  d1 == d2
来源：http://ivq.zhijiandao.cn

C#:   d1 < d2;  d1 == d2
来源：http://pqc.fktsv.cn

[J08] 提取年月日与星期
来源：http://tsd.ywan-chungtsiang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ogr.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bed.pycfn.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bxp.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kwe.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fja.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hwf.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bbm.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cvq.guowangkeji.top

[J09] 时区处理
来源：http://ljf.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bbq.zhaomingkeji.xyz


<!-- 参考信息 -->