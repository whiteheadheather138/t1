代发 wailian999

[G10] 访问控制
来源：http://bpq.feifeiyinyue.top

Py:   约定 _protected / __private（不强制）
来源：http://kyp.xingfuxueyuan.xyz

PHP:  public / protected / private
来源：http://hue.fehbvm.com

JS:   #private 字段；其余公开
来源：http://xkv.jinqigfzy.top

TS:   public / protected / private
来源：http://fqg.guannengcc.top

Java: public / protected / private / 默认包级
来源：http://tyo.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uen.jiagoushi.top

Ruby: public / protected / private
来源：http://umm.yj20258888.top

C#:   public / protected / private / internal
来源：http://osh.xylfe.cn

[G11] getter / setter
来源：http://ipu.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://bpj.sxryk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://diz.yangfankeji.com

JS:   get name() { return this._name; }
来源：http://nnk.ydzc1.top

TS:   get name(): string { return this._name; }
来源：http://hye.yueranfly.top

Java: public String getName() { return name; }
来源：http://bic.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pjn.nwbrower.top

Ruby: attr_accessor :name
来源：http://zwh.tarul.cn

C#:   public string Name { get; set; }
来源：http://fac.meibo888.top

[G12] 对象转字符串
来源：http://srl.pycfn.com

Py:   def __str__(self): return self.name
来源：http://dse.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mrz.hfpthk.cn

JS:   toString() { return this.name; }
来源：http://xcr.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://qrp.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://bpk.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://dqd.daxiang520.top

Ruby: def to_s; @name; end
来源：http://juu.xylfe.cn

C#:   public override string ToString() => Name;
来源：http://myk.chenlongwang.top

[G13] 判断对象类型
来源：http://dsy.snrcjt.cn

Py:   isinstance(u, User)
来源：http://mrh.xziqi.cn

PHP:  $u instanceof User
来源：http://itx.hammf.cn

JS:   u instanceof User
来源：http://wwi.ydzc1.top

TS:   u instanceof User
来源：http://bcx.epnwcf.com

Java: u instanceof User
来源：http://wbb.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xaf.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://sec.zhixingplan.top

C#:   u is User
来源：http://vhh.zhoulong.xyz

[G14] 数据类 / record
来源：http://pcb.havefunace.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xph.gaohongyu789.top

PHP:  // 用 readonly 属性模拟
来源：http://gvu.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vbw.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://teq.havefunace.top

Java: record User(String name, int age) {}
来源：http://bos.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://owd.nanxinkj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://unk.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://bqc.guannengcc.top

[G15] 枚举
来源：http://wqi.cashguo.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fkt.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xrk.kuanghao11.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://amh.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://btd.ivvv.top

Java: enum Color { RED, GREEN }
来源：http://elr.daxiang520.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://epa.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://ezr.wangshuangyany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://skx.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://jkh.wangshuangyany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gnj.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://lum.hywenlv.cn

JS:   Object.entries(obj)
来源：http://xdm.tanke756.top

TS:   Object.entries(obj)
来源：http://sam.jianghu66.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bse.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://uin.ppjwa.cn

Ruby: obj.instance_variables
来源：http://mif.tian-w.cn

C#:   // 用反射或 System.Text.Json
来源：http://uqa.52xcode.cn

================================================================================
来源：http://txm.9152youxi.cn

H. 异常与错误处理
来源：http://iab.xuanzx.com

================================================================================
来源：http://bul.hammf.cn

[H01] try / catch 基础
来源：http://hdl.quarkkingdee.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qgh.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iru.zycfv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pma.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qsp.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uxc.sweek.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jld.jinghuilouyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dtj.zhaomingkeji.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gcc.vehdjk.com

[H02] finally / ensure 收尾
来源：http://gpi.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://veg.sysykeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://und.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://ptw.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jcd.birdmap.top

Java: try { f(); } finally { cleanup(); }
来源：http://xjm.gogol.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ozq.shzxlz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://iri.ivvv.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://soj.xinyue.icu

[H03] 主动抛出异常
来源：http://vmn.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://ueb.pycfn.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://brx.9152youxi.cn

JS:   throw new Error("错误信息");
来源：http://nfj.jqgufenzy.top

TS:   throw new Error("错误信息");
来源：http://aqc.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://apf.tian-w.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vvw.fanxiaobao.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://orv.tarul.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zwz.svipenyu.cn

[H04] 自定义异常类型
来源：http://nwd.hesvh.cn

Py:   class MyError(Exception): pass
来源：http://yup.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://xmb.bbcook.cn

JS:   class MyError extends Error {}
来源：http://nxi.xuanzx.com

TS:   class MyError extends Error {}
来源：http://jni.kuanghao11.cn

Java: class MyException extends RuntimeException {}
来源：http://rox.sjlbkw.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gkv.daxiang520.top

Ruby: class MyError < StandardError; end
来源：http://gxn.hammf.cn

C#:   class MyException : Exception {}
来源：http://ilt.gaohongyu789.top

[H05] 捕获特定类型
来源：http://lvn.zycfv.cn

Py:   except ValueError as e:
来源：http://spj.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mbt.zhongyouzk.top

JS:   if (e instanceof TypeError) {}
来源：http://dec.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://qcv.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://blw.nanxuanxn.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pmq.yj202588.top

Ruby: rescue ArgumentError => e
来源：http://ixi.svipenyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uhw.shanyushiyangtech.top

[H06] 可选值 / 空值安全访问
来源：http://fkr.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://nda.shuidangran.top

PHP:  $v = $d["k"] ?? null;
来源：http://nim.shangyingyoupin.top

JS:   obj?.a?.b;  d ?? default
来源：http://mkg.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://orb.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ktp.guannengcc.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yxo.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://yjd.shuidangran.top

C#:   obj?.A?.B ?? default
来源：http://ajv.zhoulong.xyz

[H07] 断言
来源：http://own.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://dyr.shuidangran.top

PHP:  assert($x > 0);
来源：http://vjm.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://gse.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://odj.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://pot.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zck.feifeiyinyue.top

Ruby: raise "必须为正" unless x > 0
来源：http://nkv.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://hgh.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://mkt.yuxming.cn

Py:   str(e);  traceback.format_exc()
来源：http://kbe.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fbh.jianghu66.top

JS:   e.message;  e.stack
来源：http://ncc.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mtq.zdqjudy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yqp.daria6918.cn

Go:   err.Error()
来源：http://knr.zhixingplan.top

Ruby: e.message;  e.backtrace
来源：http://ash.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://ftu.dianchejie.cn

[H09] 带错误码的异常
来源：http://oow.sysykeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ahm.aizwys.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wvs.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kwi.jinyuanbaomall.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xzp.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tjl.52xcode.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fru.meibo888.top

Ruby: raise MyError.new("fail", 500)
来源：http://nhe.jinghuilouyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ocu.chenjidiqi.icu

[H10] 资源自动释放
来源：http://tjt.hnqzz.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dvu.bbcook.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xkr.gaohongyu789.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zyf.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jqa.guannengcc.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aan.mhx1999.top

Go:   defer f.Close()
来源：http://syb.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uax.9152youxi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lfs.daria6918.cn

================================================================================
来源：http://jmb.fengsongda.top

I. 正则表达式
来源：http://lcu.sweek.top

================================================================================
来源：http://hyk.nwbrower.top

[I01] 判断是否匹配
来源：http://yno.daxiang520.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qms.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://afg.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://fzu.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://ppb.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ejw.yongpay.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qfg.xingfuxueyuan.xyz

Ruby: s.match?(/\d+/)
来源：http://uhb.hnxiangtu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tlb.vqdsnc.cn

[I02] 提取所有匹配
来源：http://qtr.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://kqw.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://old.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vxh.yj20258.top

TS:   s.match(/\d+/g)
来源：http://ori.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://izw.sxryk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://afz.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://gja.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://slq.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://lvv.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iry.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dab.tarul.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eeq.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sln.andypj.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dyq.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://slb.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ccj.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zay.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://sdt.hywenlv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jem.daxiang520.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://scb.hnqzz.top

JS:   s.replace(/\d+/g, "#")
来源：http://abs.xuanzx.com

TS:   s.replace(/\d+/g, "#")
来源：http://etv.hnxiangtu.top

Java: s.replaceAll("\\d+", "#")
来源：http://phk.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hle.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lrx.dianchejie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://efr.xuanzx.com

[I05] 按正则拆分
来源：http://yfi.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://zrw.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mtz.sjlbkw.cn

JS:   s.split(/\s*,\s*/)
来源：http://vvl.zhoulong.xyz

TS:   s.split(/\s*,\s*/)
来源：http://qaw.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://xtb.dashuyun.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jcj.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://ajd.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kly.sxryk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zzs.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vao.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ley.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fkq.birdmap.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kzx.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nwc.gogol.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uzl.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eqf.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qao.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://ulx.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pxj.shzxlz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nwf.hesvh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jsr.zhengqikj.top

TS:   /error/gim
来源：http://rwx.ydzc1.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hug.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wsc.sjlbkw.cn

Ruby: s.scan(/error/i)
来源：http://mha.zhiwuduotai.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xel.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://ngf.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qqe.gogol.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hvb.zhijiandao.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gsd.sxryk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://trj.yangfankeji.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://amm.jinqigufen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aog.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aoc.tian-w.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://svk.svipenyu.cn

================================================================================
来源：http://huc.jqgfzy.top

J. 日期与时间
来源：http://mun.hysaishi.cn

================================================================================
来源：http://auj.xingfuxueyuan.xyz

[J01] 获取当前时间
来源：http://alg.ppjwa.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ydq.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mzt.tian-w.cn

JS:   new Date();  Date.now()
来源：http://qxs.bbcook.cn

TS:   new Date();  Date.now()
来源：http://cle.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uwn.tarul.cn

Go:   time.Now()
来源：http://uby.fanxiaobao.xyz

Ruby: Time.now
来源：http://ixd.tanke756.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uit.shanyushiyangkeji.top

[J02] 格式化输出
来源：http://xpy.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tgj.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dno.chenlongwang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rvq.zdqjudy.top

TS:   d.toISOString()
来源：http://vjj.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ujw.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kps.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tza.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://izi.ydzc1.top

[J03] 字符串解析为日期
来源：http://ckx.yj20258888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ccx.hnqzz.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wno.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://ene.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://cvl.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://kxq.tanke756.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vji.sweek.top

Ruby: Date.parse("2024-01-02")
来源：http://wtw.yuxming.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kpl.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://lig.andypj.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hdh.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kdb.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://asw.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zcm.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vmx.zdbjq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sro.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ytc.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://azb.gzhubu.top

[J05] 时间加减（加 7 天）
来源：http://loh.hnxiangtu.top

Py:   now + timedelta(days=7)
来源：http://icq.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://iks.zhijiandao.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://twe.zhixingplan.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ade.smart0.xyz

Java: LocalDate.now().plusDays(7)
来源：http://pvc.tianlin.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ehw.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://otl.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sxb.sufxvd.cn

[J06] 计算两时间之差
来源：http://ywj.uphjek.com

Py:   (end - start).total_seconds()
来源：http://prv.yj20258.top

PHP:  $end->diff($start)->days;
来源：http://uvl.hnqzz.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cbv.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xrl.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mjy.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://rhq.ybcxt.top

Ruby: end - start                 # 返回秒数
来源：http://ubc.daxiang520.top

C#:   (end - start).TotalSeconds
来源：http://ant.jqgufenzy.top

[J07] 比较两个日期
来源：http://rkj.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://ejf.ydjk.org.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hrs.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://gus.yuxming.cn

TS:   d1.getTime() < d2.getTime()
来源：http://knr.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ioe.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fjh.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://usu.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://cvc.daxiang520.top

[J08] 提取年月日与星期
来源：http://kdc.zdbjq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ppa.ywan-chungtsiang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://byz.daxiang520.top


<!-- 参考信息 -->