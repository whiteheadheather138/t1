代发 wailian999

TS:   public / protected / private
来源：http://wrn.316326.xyz

Java: public / protected / private / 默认包级
来源：http://fgh.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dse.xuanzx.com

Ruby: public / protected / private
来源：http://gfh.hysaishi.cn

C#:   public / protected / private / internal
来源：http://hgk.sufxvd.cn

[G11] getter / setter
来源：http://kxp.fktsv.cn

Py:   @property 与 @x.setter
来源：http://tzj.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qyz.aizwys.cn

JS:   get name() { return this._name; }
来源：http://tiv.hongshengwenyu.top

TS:   get name(): string { return this._name; }
来源：http://xpg.nwbrower.top

Java: public String getName() { return name; }
来源：http://dvu.yonumen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://blw.hywenlv.cn

Ruby: attr_accessor :name
来源：http://mkz.iojbl.cn

C#:   public string Name { get; set; }
来源：http://lzr.shangyingyoupin.top

[G12] 对象转字符串
来源：http://its.yj202588.top

Py:   def __str__(self): return self.name
来源：http://ske.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://czn.cashguo.top

JS:   toString() { return this.name; }
来源：http://evv.jyoumei.cn

TS:   toString(): string { return this.name; }
来源：http://jyc.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://vyh.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://hxy.vehdjk.com

Ruby: def to_s; @name; end
来源：http://faj.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://ukh.haohaochexian.top

[G13] 判断对象类型
来源：http://umo.gogol.net.cn

Py:   isinstance(u, User)
来源：http://dnx.fengsongda.top

PHP:  $u instanceof User
来源：http://dnr.guannengcc.top

JS:   u instanceof User
来源：http://vky.bbcook.cn

TS:   u instanceof User
来源：http://qmj.shzxlz.cn

Java: u instanceof User
来源：http://dey.yueranfly.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://prx.cqqwz.cn

Ruby: u.is_a?(User)
来源：http://cuk.yfazqb.com

C#:   u is User
来源：http://mfo.cqqwz.cn

[G14] 数据类 / record
来源：http://xnf.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fsy.wangdashe.top

PHP:  // 用 readonly 属性模拟
来源：http://fvi.xuanzx.com

JS:   // 无内置：普通类或对象字面量
来源：http://ooh.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://euw.fktsv.cn

Java: record User(String name, int age) {}
来源：http://nlc.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://zko.yj202588.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cco.ppjwa.cn

C#:   record User(string Name, int Age);
来源：http://apz.fengsongda.top

[G15] 枚举
来源：http://hem.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nzq.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wod.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kno.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://osp.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://krk.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://klz.ppjwa.cn

Ruby: Color = %i[red green].freeze
来源：http://uhi.yanxiufei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pbg.havefunace.top

[G16] 对象转数组 / 字典
来源：http://mnd.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yhx.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://cdb.gzhubu.top

JS:   Object.entries(obj)
来源：http://doc.dianchejie.cn

TS:   Object.entries(obj)
来源：http://yvb.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dmm.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tze.xinyue.icu

Ruby: obj.instance_variables
来源：http://gnk.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://ahx.zhengqikj.top

================================================================================
来源：http://kvg.yongpay.top

H. 异常与错误处理
来源：http://mvk.tanke756.top

================================================================================
来源：http://mlp.aizwys.cn

[H01] try / catch 基础
来源：http://yfh.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dox.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tch.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xbd.yueranfly.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hbi.nwbrower.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lcg.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://okc.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cft.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iez.ybcxt.top

[H02] finally / ensure 收尾
来源：http://apl.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kuo.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://quq.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ysd.sweek.top

TS:   try { f(); } finally { cleanup(); }
来源：http://olb.yuanzhike.top

Java: try { f(); } finally { cleanup(); }
来源：http://gkm.0kj1m.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qwe.guowangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bti.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xfz.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://uqc.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://zsf.wangshuangyany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wnt.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://pbd.xuetiantiany.cn

TS:   throw new Error("错误信息");
来源：http://zcr.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wai.hcnkem.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vdd.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pwc.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://gqw.birdmap.top

[H04] 自定义异常类型
来源：http://tbm.andypj.xyz

Py:   class MyError(Exception): pass
来源：http://kvk.redwolf501.top

PHP:  class MyError extends RuntimeException {}
来源：http://vhv.smart0.xyz

JS:   class MyError extends Error {}
来源：http://poa.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://vlx.nanxinkj.top

Java: class MyException extends RuntimeException {}
来源：http://btv.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uwc.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://uoc.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://cbg.pengpengdd.cyou

[H05] 捕获特定类型
来源：http://yqu.xuetiantiany.cn

Py:   except ValueError as e:
来源：http://odl.kuanghao11.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wez.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://qvr.jqgfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://fli.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://apr.tanke756.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vnj.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://avv.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mur.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://era.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://oii.gzhubu.top

PHP:  $v = $d["k"] ?? null;
来源：http://ips.pycfn.com

JS:   obj?.a?.b;  d ?? default
来源：http://fsm.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://mcx.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qbv.andypj.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://cbv.jianghu66.top

Ruby: d&.dig(:a, :b)
来源：http://gwz.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://dzc.uphjek.com

[H07] 断言
来源：http://mya.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://tfv.xuetiantiany.cn

PHP:  assert($x > 0);
来源：http://gbm.tanke756.top

JS:   console.assert(x > 0);
来源：http://cnr.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://cal.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://qbb.xylfe.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rlv.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ztq.yonumen.top

C#:   Debug.Assert(x > 0);
来源：http://vdb.sjlbkw.cn

[H08] 获取错误信息与堆栈
来源：http://jnz.bjfxy.top

Py:   str(e);  traceback.format_exc()
来源：http://quh.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ekc.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://gtu.zhengqikj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://spl.hammf.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nxn.aibaodan.cn

Go:   err.Error()
来源：http://gus.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://klz.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://wlb.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://xqa.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cgf.hesvh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xaf.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ktr.jinqigufen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wkr.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cqi.aizwys.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ghr.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://zju.bbcook.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://obh.jyoumei.cn

[H10] 资源自动释放
来源：http://wsq.pycfn.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://mfw.tian-w.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://win.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xvn.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ept.hongshengwenyu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ezl.haohaochexian.top

Go:   defer f.Close()
来源：http://zzl.cheryme.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jne.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nhj.ybcxt.top

================================================================================
来源：http://dch.cdnleiting.top

I. 正则表达式
来源：http://yxw.gaohongyu789.top

================================================================================
来源：http://vkz.xinyue.icu

[I01] 判断是否匹配
来源：http://wms.sxryk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://col.iojbl.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tnw.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://qeo.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://vsr.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fzh.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qul.yj20258.top

Ruby: s.match?(/\d+/)
来源：http://brk.mhx1999.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wbb.cqqwz.cn

[I02] 提取所有匹配
来源：http://pmf.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://xqi.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://obk.52xcode.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eyt.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://azw.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wha.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fle.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://sao.yanxiufei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://esw.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://hly.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sem.uphjek.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zox.jinyuanbaomall.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sft.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mxc.bjfxy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://slr.kuanghao11.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://usm.sweek.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yrs.zdbjq.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tyn.yueranfly.top

[I04] 正则替换
来源：http://axj.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nnf.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vmc.iojbl.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vbq.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://akz.jiagoushi.top

Java: s.replaceAll("\\d+", "#")
来源：http://ndx.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yfs.zdqjudy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uaa.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kfj.ivvv.top

[I05] 按正则拆分
来源：http://bad.bbcook.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uiw.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jxh.ywan-chungtsiang.top

JS:   s.split(/\s*,\s*/)
来源：http://obv.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://zct.jinyuanbaomall.cn

Java: s.split("\\s*,\\s*")
来源：http://pmm.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://imt.zhixingplan.top

Ruby: s.split(/\s*,\s*/)
来源：http://zhb.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ymd.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wyj.ivvv.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vbv.xylfe.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ejo.cashguo.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nrm.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vhs.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vcd.yfazqb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://otu.hesvh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zpq.fzhhl.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ejd.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://qts.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qnv.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dmp.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://djo.cheryme.top

TS:   /error/gim
来源：http://iwr.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ocp.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oxg.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://ubc.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yyo.hnqzz.top

[I08] 贪婪与非贪婪匹配
来源：http://qzx.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bnl.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lsu.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ylw.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gzc.jinqigfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oda.svipenyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tuu.hfpthk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ray.gzhubu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sgu.52xcode.cn

================================================================================
来源：http://cwf.fktsv.cn

J. 日期与时间
来源：http://paf.ivvv.top

================================================================================
来源：http://krg.yueranfly.top

[J01] 获取当前时间
来源：http://xub.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dld.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fkz.tian-w.cn

JS:   new Date();  Date.now()
来源：http://ieg.shanyushiyangtech.top

TS:   new Date();  Date.now()
来源：http://bgx.nwbrower.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vry.zdbjq.cn

Go:   time.Now()
来源：http://rco.yj20258.top

Ruby: Time.now
来源：http://rse.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gta.hnqzz.top

[J02] 格式化输出
来源：http://iee.sjlbkw.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dwh.ydjk.org.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fkp.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ray.gogol.net.cn

TS:   d.toISOString()
来源：http://qau.dashuyun.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wtr.yj20258.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hhd.uphjek.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rnb.pycfn.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hio.sweek.top

[J03] 字符串解析为日期
来源：http://gik.yj202588.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oeu.zhengqikj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ndj.chenjidiqi.icu

JS:   new Date("2024-01-02")
来源：http://wmr.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://lyb.xingfuxueyuan.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://rqv.hfpthk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zze.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://khs.jianghu66.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sjg.52xcode.cn

[J04] 时间戳与日期互转
来源：http://jgm.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sbh.daria6918.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bxt.redwolf501.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qay.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://int.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dpy.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://chz.cashguo.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yiy.52xcode.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wfr.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://stb.yvedp.cn

Py:   now + timedelta(days=7)
来源：http://ukh.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qdt.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fkc.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ywh.nwbrower.top

Java: LocalDate.now().plusDays(7)
来源：http://fkr.tanke756.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dyb.hongshengwenyu.top

Ruby: Time.now + 7 * 86400
来源：http://ccp.tarul.cn

C#:   DateTime.Now.AddDays(7)
来源：http://owc.smart0.xyz

[J06] 计算两时间之差
来源：http://zyo.hnxiangtu.top

Py:   (end - start).total_seconds()
来源：http://wjf.daxiang520.top

PHP:  $end->diff($start)->days;
来源：http://tfe.zhaomingkeji.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aei.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://apq.uphjek.com

Java: Duration.between(start, end).toSeconds()
来源：http://tia.zhixingplan.top

Go:   end.Sub(start).Hours()
来源：http://oog.chenjidiqi.icu

Ruby: end - start                 # 返回秒数
来源：http://ntx.ywan-chungtsiang.top

C#:   (end - start).TotalSeconds
来源：http://hub.aizwys.cn

[J07] 比较两个日期
来源：http://yra.redwolf501.top

Py:   d1 < d2;  d1 == d2
来源：http://xyr.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dbm.9152youxi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vaj.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://pjq.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fje.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gxj.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://ppy.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://cre.iojbl.cn

[J08] 提取年月日与星期
来源：http://opj.zhaomingkeji.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://har.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gpv.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ico.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jvp.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lep.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tsf.hysaishi.cn


<!-- 参考信息 -->