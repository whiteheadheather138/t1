代发 wailian999

[Q63] 开启事务
来源：http://ocy.bbcook.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://plq.shuidangran.top

[Q64] 提交事务
来源：http://nwv.zhixingplan.top

COMMIT;
来源：http://wrc.zhengqikj.top

[Q65] 回滚事务
来源：http://epq.guowangkeji.top

ROLLBACK;
来源：http://cay.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://rxr.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vrr.yj20258888.top

[Q67] 设置隔离级别
来源：http://dbk.cashguo.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bqv.gaohongyu789.top

[Q68] 保存点
来源：http://bqy.yj202588.top

SAVEPOINT sp1;
来源：http://jmg.yuanzhike.top

ROLLBACK TO sp1;
来源：http://ews.quarkkingdee.top

[Q69] 查看执行计划
来源：http://ipy.iojbl.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pdp.bbcook.cn

[Q70] 更新统计信息
来源：http://eld.hammf.cn

ANALYZE TABLE users;
来源：http://fbb.cqqwz.cn

[Q71] 查看建表语句
来源：http://txw.cashguo.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nng.yonumen.top

[Q72] 查看索引
来源：http://sof.tarul.cn

SHOW INDEX FROM users;
来源：http://hxw.pengpengdd.cyou

[Q73] 查看表状态
来源：http://ndy.xziqi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cwt.zdbjq.cn

[Q74] 强制使用索引
来源：http://qbe.c1oappe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bgp.nanxuanxn.top

[Q75] 日期格式化
来源：http://psa.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kwg.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://obl.andypj.xyz

[Q76] 按天统计
来源：http://pwe.shangyingyoupin.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://unl.epnwcf.com

[Q77] 时间加减
来源：http://kvd.hcnkem.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mbc.yfazqb.com

[Q78] 当前时间
来源：http://chw.zhijiandao.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://czs.vqdsnc.cn

[Q79] 字符串拼接
来源：http://slv.hysaishi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oke.nwbrower.top

[Q80] 字符串截取
来源：http://jpb.kuanghao11.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rld.sxryk.cn

[Q81] 字符串替换
来源：http://fvr.jianghu66.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ips.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://dfw.shanyushiyangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vfm.cqqwz.cn

[Q83] 大小写转换
来源：http://lkj.0kj1m.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rvi.vehdjk.com

[Q84] 去除首尾空格
来源：http://tuv.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://lxs.vqdsnc.cn

[Q85] 数值取整
来源：http://rfb.ydjk.org.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qvd.c1oappe.top

[Q86] 读取 JSON 字段
来源：http://jnu.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://quz.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://cfb.tanke756.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yrk.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://gcx.redwolf501.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mbl.jiagoushi.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tnk.gotoacloud.top

[Q89] 判断表是否存在
来源：http://oni.hysaishi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ecr.hesvh.cn

[Q90] 生成序号列
来源：http://nbj.jinqigufen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vvc.ywan-chungtsiang.top

================================================================================
来源：http://kss.xziqi.cn

R. Bash 专题
来源：http://nyo.wangdashe.top

================================================================================
来源：http://qas.sweek.top

[R01] shebang 与严格模式
来源：http://hki.dianchejie.cn

#!/usr/bin/env bash
来源：http://abn.ydjk.org.cn

set -euo pipefail
来源：http://egt.birdmap.top

[R02] 变量赋值与使用
来源：http://dal.ydjk.org.cn

name="Tom"; echo "$name"
来源：http://sfa.gzhubu.top

[R03] 只读变量
来源：http://zqx.jinqigfzy.top

readonly PI=3.14
来源：http://lgd.sysykeji.top

[R04] 位置参数
来源：http://ulr.iojbl.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ala.yanxiufei.cn

[R05] 参数默认值
来源：http://ibw.guowangkeji.top

name="${1:-default}"
来源：http://vrv.ybcxt.top

[R06] 判断命令是否存在
来源：http://kwf.chenjidiqi.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cyo.chenzaomai.com

[R07] if 判断文件
来源：http://fpn.zdbjq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xtg.smart0.xyz

[R08] 数值比较
来源：http://jts.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hpz.ctjpmb.com

[R09] 字符串比较
来源：http://ved.9152youxi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ysw.yvedp.cn

[R10] 正则匹配
来源：http://fcd.yj20258888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://txk.yuanzhike.top

[R11] case 多分支
来源：http://uzf.havefunace.top

case "$1" in
来源：http://xrp.xuetiantiany.cn

start) echo "启动" ;;
来源：http://sfc.jinqigfzy.top

stop)  echo "停止" ;;
来源：http://lhv.ydjk.org.cn

*)     echo "未知命令" ;;
来源：http://met.yuxming.cn

esac
来源：http://kfd.havefunace.top

[R12] for 遍历文件
来源：http://fgu.bbcook.cn

for f in *.txt; do echo "$f"; done
来源：http://swz.yongpay.top

[R13] for 计数循环
来源：http://jrq.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://mkt.yuxming.cn

[R14] C 风格 for
来源：http://vkt.hywenlv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dih.ybcxt.top

[R15] while 逐行读文件
来源：http://ujs.yj202588.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cwm.52xcode.cn

[R16] until 等待条件
来源：http://pqf.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cfc.jqgfzy.top

[R17] 数组定义与取值
来源：http://dsa.ppjwa.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yhv.quarkkingdee.top

[R18] 遍历数组
来源：http://hwq.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wzv.chenlongwang.top

[R19] 数组长度
来源：http://jss.zhixingplan.top

echo "${#arr[@]}"
来源：http://gta.cheryme.top

[R20] 关联数组（字典）
来源：http://jln.pycfn.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tyq.tian-w.cn

[R21] 字符串长度
来源：http://wxf.fzhhl.top

echo "${#s}"
来源：http://sbc.yuxming.cn

[R22] 截取子串
来源：http://anc.iojbl.cn

echo "${s:0:5}"
来源：http://wyp.aibaodan.cn

[R23] 字符串替换
来源：http://rwf.ppjwa.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://unw.meibo888.top

[R24] 大小写转换
来源：http://qyi.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://loj.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://bci.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://snw.meibo888.top

[R26] 命令替换
来源：http://unq.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://mkz.gzhubu.top

[R27] 算术展开
来源：http://gly.jinqigufen.top

echo $((1 + 2 * 3))
来源：http://qox.hnqzz.top

[R28] 浮点运算
来源：http://hmf.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://xbv.gogol.net.cn

[R29] 定义函数
来源：http://cfo.xuetiantiany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lfb.epnwcf.com

[R30] 函数返回状态码
来源：http://das.xuetiantiany.cn

f() { return 0; }; f || echo "失败了"
来源：http://ypy.zdbjq.cn

[R31] 局部变量
来源：http://kii.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://xlo.jinqigfzy.top

[R32] 参数个数校验
来源：http://tzr.mhx1999.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vqv.chenlongwang.top

[R33] 捕获错误并提示行号
来源：http://sqr.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uvu.birdmap.top

[R34] 退出时清理
来源：http://hgb.jlsjyb.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nkh.haohaochexian.top

[R35] 后台执行并等待
来源：http://mdt.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iso.9152youxi.cn

[R36] 并发执行多个任务
来源：http://ior.ydzc1.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kxe.mhx1999.top

[R37] 把输出赋给变量
来源：http://wvg.daria6918.cn

files=$(ls -1)
来源：http://cxa.tianlin.xyz

[R38] 管道串联
来源：http://tho.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://art.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://nko.snrcjt.cn

cmd > out.log 2>&1
来源：http://ahs.hysaishi.cn

[R40] 追加写日志
来源：http://vhm.aibaodan.cn

echo "log" >> out.log
来源：http://ouf.sjlbkw.cn

[R41] 丢弃输出
来源：http://zpw.vehdjk.com

cmd >/dev/null 2>&1
来源：http://aco.hnxiangtu.top

[R42] 输入重定向
来源：http://gzu.yonumen.top

wc -l < a.txt
来源：http://anq.zhiwuduotai.top

[R43] 按名字查找文件
来源：http://hlh.bjfxy.top

find . -name "*.log" -type f
来源：http://rze.hesvh.cn

[R44] 按修改时间查找
来源：http://jyt.nanxinkj.top

find . -mtime -7 -type f
来源：http://uah.ydzc1.top

[R45] 批量删除
来源：http://zmr.pengpengdd.cyou

find . -name "*.tmp" -delete
来源：http://emv.iojbl.cn

[R46] 递归替换文件内容
来源：http://sgx.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yeh.wangdashe.top

[R47] sed 单行替换
来源：http://mol.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kdh.gaohongyu789.top

[R48] awk 取指定列
来源：http://qbp.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://vgm.pycfn.com

[R49] awk 带条件
来源：http://ues.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aal.jinghuilouyu.cn

[R50] awk 求和
来源：http://kax.fanxiaobao.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://bbm.shzxlz.cn

[R51] 排序去重取前几
来源：http://mkm.jlsjyb.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nsa.gzhubu.top

[R52] 统计行数
来源：http://glm.cdnleiting.top

wc -l a.txt
来源：http://qdb.zycfv.cn

[R53] 查看文件头与实时尾
来源：http://bxs.daria6918.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xqx.tarul.cn

[R54] 比较两个文件
来源：http://jqq.xinyue.icu

diff a.txt b.txt
来源：http://zdj.yj202588.top

[R55] 压缩与解压
来源：http://msc.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iya.xinyue.icu

[R56] 远程拷贝
来源：http://zzg.aibaodan.cn

scp file user@host:/path/
来源：http://ljx.hfpthk.cn

[R57] 远程执行命令
来源：http://wwx.chenjidiqi.icu

ssh user@host 'uptime'
来源：http://grb.haohaochexian.top

[R58] 下载文件
来源：http://kdd.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qlp.yj20258.top

[R59] 发 POST JSON
来源：http://byw.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jrp.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://rkz.tarul.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://plz.ybcxt.top

[R61] 磁盘占用
来源：http://inc.nwbrower.top

df -h;  du -sh *
来源：http://hat.xuanzx.com

[R62] 找最占空间的文件
来源：http://lwk.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://bey.smart0.xyz

[R63] 内存与进程
来源：http://koe.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://xfw.nanxuanxn.top

[R64] 结束进程
来源：http://fsc.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://wtd.yonumen.top

[R65] 查看端口占用
来源：http://zlz.yangfankeji.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gaq.xuetiantiany.cn

[R66] 定时任务
来源：http://ehl.xingfuxueyuan.xyz

crontab -e;  crontab -l
来源：http://chy.yj20258888.top

[R67] 生成随机十六进制串
来源：http://yeu.ctjpmb.com

openssl rand -hex 16
来源：http://zeo.jyoumei.cn

[R68] 计算文件校验值
来源：http://zgm.smart0.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://ipm.shanyushiyangtech.top

[R69] 生成随机密码
来源：http://uoc.epnwcf.com

head -c 16 /dev/urandom | base64
来源：http://zeh.vqdsnc.cn

[R70] 时间戳与互转
来源：http://fxm.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://ifs.yj202588.top

[R71] 日期格式化
来源：http://lsm.52xcode.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eeq.fehbvm.com

[R72] 等待端口就绪
来源：http://qvd.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ngx.chenjidiqi.icu

[R73] 分割大日志
来源：http://gxz.xuanzx.com

split -l 1000 big.log part_
来源：http://htt.ehwqpu.com

[R74] 批量重命名
来源：http://fub.52xcode.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aqf.zdqjudy.top

[R75] 导出环境变量
来源：http://cuk.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://ypj.zhiwuduotai.top

[R76] 使用临时文件
来源：http://uhs.zdqjudy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://adi.sysykeji.top

[R77] 读取用户输入
来源：http://kzh.yueranfly.top

read -rp "请输入: " ans
来源：http://ukr.pycfn.com

[R78] 交互式菜单
来源：http://bbl.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hjg.hnxiangtu.top

[R79] 解析命令行选项
来源：http://jym.svipenyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kvi.hammf.cn

[R80] 查看脚本执行耗时
来源：http://mif.tian-w.cn

time ./run.sh
来源：http://rli.ehwqpu.com

================================================================================
来源：http://mrv.aibaodan.cn

S. C / C++ 专题
来源：http://isp.yvedp.cn

================================================================================
来源：http://eda.birdmap.top

[S01] C：Hello World
来源：http://zgw.cashguo.top

#include <stdio.h>
来源：http://had.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kmv.yanxiufei.cn

[S02] C：变量与格式化输出
来源：http://dkt.jinqigufen.top

int a = 10; printf("%d\n", a);
来源：http://snw.hesvh.cn

[S03] C：读入整数
来源：http://rrq.zhixingplan.top

int x; scanf("%d", &x);
来源：http://yph.52xcode.cn

[S04] C：字符串复制
来源：http://oug.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://wik.yanxiufei.cn

[S05] C：字符串长度
来源：http://kps.tarul.cn

strlen(s)
来源：http://jou.jlsjyb.cn

[S06] C：字符串比较
来源：http://ysh.cqqwz.cn

strcmp(a, b) == 0
来源：http://jzk.9152youxi.cn

[S07] C：数组遍历求和
来源：http://fuq.cashguo.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qlh.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://hvi.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yhz.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://ccm.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lux.sysykeji.top

[S10] C：指针与解引用
来源：http://rbk.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://uxc.meibo888.top

[S11] C：逐行读文件
来源：http://djp.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://hwp.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ewj.fanxiaobao.xyz

fclose(f);
来源：http://twj.shanyushiyangkeji.top

[S12] C：写文件
来源：http://wzo.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rop.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://jkx.shuidangran.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://weq.ehwqpu.com

[S14] C：枚举
来源：http://qlw.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://enm.yfazqb.com

[S15] C：类型转换
来源：http://ahb.yfazqb.com

(double) a / b
来源：http://nzf.ehwqpu.com

[S16] C：位操作置位
来源：http://vmr.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://asm.sxryk.cn

[S17] C：安全拼接字符串
来源：http://wrf.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ipx.zhiwuduotai.top

[S18] C：命令行参数
来源：http://wyb.jqgufenzy.top

int main(int argc, char **argv)
来源：http://kpr.sufxvd.cn

[S19] C：快速排序
来源：http://loc.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gmf.jinqigufen.top

[S20] C：二分查找
来源：http://dmy.zhiwuduotai.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://omp.hnxiangtu.top

[S21] C：字符类别判断
来源：http://mux.fehbvm.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ywv.hesvh.cn

[S22] C：字符串转数字
来源：http://tkf.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://cti.hysaishi.cn

[S23] C：随机数
来源：http://tkw.sysykeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vca.sweek.top

[S24] C：获取本地时间
来源：http://xne.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://htd.jiagoushi.top

[S25] C：内存拷贝
来源：http://yzn.gzhubu.top

memcpy(dst, src, n);
来源：http://jpv.xuetiantiany.cn

[S26] C：内存清零
来源：http://oyu.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://bwz.shuidangran.top

[S27] C：定义常量
来源：http://waa.quarkkingdee.top

const double PI = 3.14159;
来源：http://lre.jqgufenzy.top

[S28] C：静态变量
来源：http://dsy.guowangkeji.top

static int counter = 0;
来源：http://msw.yuxming.cn

[S29] C：变参函数
来源：http://ylo.zdqjudy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jaz.epnwcf.com

[S30] C：头文件保护
来源：http://rfz.gaohongyu789.top

#ifndef X_H
来源：http://qsa.gogol.net.cn

#define X_H
来源：http://ekj.mhx1999.top

#endif
来源：http://ocj.quarkkingdee.top

[S31] C++：Hello World
来源：http://jtd.ybcxt.top

#include <iostream>
来源：http://vzs.tarul.cn

int main() { std::cout << "Hello\n"; }
来源：http://znr.jlsjyb.cn

[S32] C++：字符串
来源：http://mxk.jinqigufen.top

std::string s = "hi";  s += "!";
来源：http://adn.cqqwz.cn


<!-- 参考信息 -->