代发 wailian999

ROLLBACK TO sp1;
来源：http://hkc.shanyushiyangtech.top

[Q69] 查看执行计划
来源：http://jku.vehdjk.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eco.birdmap.top

[Q70] 更新统计信息
来源：http://yya.gotoacloud.top

ANALYZE TABLE users;
来源：http://pjm.yueranfly.top

[Q71] 查看建表语句
来源：http://wqo.meibo888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://toa.jlsjyb.cn

[Q72] 查看索引
来源：http://cid.ywan-chungtsiang.top

SHOW INDEX FROM users;
来源：http://aqn.dianchejie.cn

[Q73] 查看表状态
来源：http://tsh.hammf.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rev.gaohongyu789.top

[Q74] 强制使用索引
来源：http://dei.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ecg.gzhubu.top

[Q75] 日期格式化
来源：http://fyj.zdqjudy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nnd.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lns.yj202588.top

[Q76] 按天统计
来源：http://ctn.gotoacloud.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lae.yj20258888.top

[Q77] 时间加减
来源：http://vdq.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qmv.zhongyouzk.top

[Q78] 当前时间
来源：http://edf.jinyuanbaomall.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://urj.sxryk.cn

[Q79] 字符串拼接
来源：http://tpi.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pdt.hammf.cn

[Q80] 字符串截取
来源：http://vmo.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dpi.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://gox.fktsv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rrl.ybcxt.top

[Q82] 字符长度与字节长度
来源：http://wip.shanyushiyangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gmj.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://ulo.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zor.zhixingplan.top

[Q84] 去除首尾空格
来源：http://oxr.sxryk.cn

SELECT TRIM(name) FROM users;
来源：http://vpp.jyoumei.cn

[Q85] 数值取整
来源：http://oth.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kgy.ybcxt.top

[Q86] 读取 JSON 字段
来源：http://eij.fzhhl.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gdn.chenzaomai.com

[Q87] JSON 字段做条件
来源：http://okg.wangdashe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cqt.meibo888.top

[Q88] 行转列（条件聚合）
来源：http://qrd.zhaomingkeji.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rab.daria6918.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://udn.svipenyu.cn

[Q89] 判断表是否存在
来源：http://kvs.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bbu.cqqwz.cn

[Q90] 生成序号列
来源：http://dgf.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ecy.aibaodan.cn

================================================================================
来源：http://jhu.gotoacloud.top

R. Bash 专题
来源：http://pul.gaohongyu789.top

================================================================================
来源：http://eer.yonumen.top

[R01] shebang 与严格模式
来源：http://bnt.yonumen.top

#!/usr/bin/env bash
来源：http://fmf.c1oappe.top

set -euo pipefail
来源：http://iun.316326.xyz

[R02] 变量赋值与使用
来源：http://zmo.zhaomingkeji.xyz

name="Tom"; echo "$name"
来源：http://zvh.fanxiaobao.xyz

[R03] 只读变量
来源：http://kyw.hammf.cn

readonly PI=3.14
来源：http://tdb.jqgufenzy.top

[R04] 位置参数
来源：http://goj.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://seo.xziqi.cn

[R05] 参数默认值
来源：http://zif.sweek.top

name="${1:-default}"
来源：http://muc.feifeiyinyue.top

[R06] 判断命令是否存在
来源：http://gdp.hcnkem.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kag.hywenlv.cn

[R07] if 判断文件
来源：http://gzj.yonumen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dnp.fanxiaobao.xyz

[R08] 数值比较
来源：http://hlj.tian-w.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://abm.smart0.xyz

[R09] 字符串比较
来源：http://doe.cqqwz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cle.ppjwa.cn

[R10] 正则匹配
来源：http://xhw.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oas.dianchejie.cn

[R11] case 多分支
来源：http://omu.tanke756.top

case "$1" in
来源：http://sjg.yj20258.top

start) echo "启动" ;;
来源：http://maw.shangyingyoupin.top

stop)  echo "停止" ;;
来源：http://qof.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://iea.uphjek.com

esac
来源：http://jzi.kuanghao11.cn

[R12] for 遍历文件
来源：http://zds.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://qna.c1oappe.top

[R13] for 计数循环
来源：http://rhy.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://xlh.ehwqpu.com

[R14] C 风格 for
来源：http://jfw.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://agj.hnqzz.top

[R15] while 逐行读文件
来源：http://cdp.birdmap.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dts.kuanghao11.cn

[R16] until 等待条件
来源：http://eci.sweek.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://guz.yueranfly.top

[R17] 数组定义与取值
来源：http://gbq.fengsongda.top

arr=(a b c); echo "${arr[0]}"
来源：http://pmu.birdmap.top

[R18] 遍历数组
来源：http://kch.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nvv.jinqigfzy.top

[R19] 数组长度
来源：http://fbg.jinqigufen.top

echo "${#arr[@]}"
来源：http://ctp.snrcjt.cn

[R20] 关联数组（字典）
来源：http://agt.zycfv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kks.jinqigfzy.top

[R21] 字符串长度
来源：http://seb.pengpengdd.cyou

echo "${#s}"
来源：http://wgd.hywenlv.cn

[R22] 截取子串
来源：http://zzi.yj20258.top

echo "${s:0:5}"
来源：http://oxw.jinqigfzy.top

[R23] 字符串替换
来源：http://fqa.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wfj.zhoulong.xyz

[R24] 大小写转换
来源：http://uxu.cdnleiting.top

echo "${s^^}"; echo "${s,,}"
来源：http://qra.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://vkd.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ajn.vehdjk.com

[R26] 命令替换
来源：http://izs.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://swn.quarkkingdee.top

[R27] 算术展开
来源：http://clg.zhengqikj.top

echo $((1 + 2 * 3))
来源：http://pij.zhixingplan.top

[R28] 浮点运算
来源：http://fbf.shanyushiyangkeji.top

echo "scale=2; 10/3" | bc
来源：http://hdb.shanyushiyangkeji.top

[R29] 定义函数
来源：http://qqt.wangdashe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vna.fengsongda.top

[R30] 函数返回状态码
来源：http://hxs.zhoulong.xyz

f() { return 0; }; f || echo "失败了"
来源：http://hqb.meibo888.top

[R31] 局部变量
来源：http://uwu.fzhhl.top

f() { local x=1; echo "$x"; }
来源：http://lxp.chenzaomai.com

[R32] 参数个数校验
来源：http://hfx.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pvu.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://xyh.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pih.shzxlz.cn

[R34] 退出时清理
来源：http://csl.ywan-chungtsiang.top

trap 'rm -f "$tmp"' EXIT
来源：http://vca.tarul.cn

[R35] 后台执行并等待
来源：http://syb.ehwqpu.com

sleep 5 & pid=$!; wait "$pid"
来源：http://fjs.chenzaomai.com

[R36] 并发执行多个任务
来源：http://led.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zjs.haohaochexian.top

[R37] 把输出赋给变量
来源：http://xsb.xinyue.icu

files=$(ls -1)
来源：http://jve.sjlbkw.cn

[R38] 管道串联
来源：http://btm.ivvv.top

cat a.txt | grep -i error | wc -l
来源：http://fbd.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://qdg.zycfv.cn

cmd > out.log 2>&1
来源：http://zzs.yonumen.top

[R40] 追加写日志
来源：http://nsn.tian-w.cn

echo "log" >> out.log
来源：http://sem.52xcode.cn

[R41] 丢弃输出
来源：http://yxf.andypj.xyz

cmd >/dev/null 2>&1
来源：http://gjf.gogol.net.cn

[R42] 输入重定向
来源：http://tku.cucudq.cn

wc -l < a.txt
来源：http://xea.shuidangran.top

[R43] 按名字查找文件
来源：http://rls.sysykeji.top

find . -name "*.log" -type f
来源：http://ryp.zhoulong.xyz

[R44] 按修改时间查找
来源：http://eul.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://xes.xziqi.cn

[R45] 批量删除
来源：http://rgl.shzxlz.cn

find . -name "*.tmp" -delete
来源：http://cxn.pengpengdd.cyou

[R46] 递归替换文件内容
来源：http://sxu.jinghuilouyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uol.hysaishi.cn

[R47] sed 单行替换
来源：http://ine.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lze.dianchejie.cn

[R48] awk 取指定列
来源：http://kvy.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://sah.hfpthk.cn

[R49] awk 带条件
来源：http://ush.cashguo.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pvr.gogol.net.cn

[R50] awk 求和
来源：http://kxx.fktsv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bzm.gotoacloud.top

[R51] 排序去重取前几
来源：http://sdv.cheryme.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fjj.fzhhl.top

[R52] 统计行数
来源：http://rts.vqdsnc.cn

wc -l a.txt
来源：http://mve.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://jwh.hywenlv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://imt.mhx1999.top

[R54] 比较两个文件
来源：http://cjr.kuanghao11.cn

diff a.txt b.txt
来源：http://dgd.nanxuanxn.top

[R55] 压缩与解压
来源：http://qyf.fehbvm.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yjl.fzhhl.top

[R56] 远程拷贝
来源：http://csm.yj20258.top

scp file user@host:/path/
来源：http://pqg.hammf.cn

[R57] 远程执行命令
来源：http://bzz.cashguo.top

ssh user@host 'uptime'
来源：http://wgq.chenzaomai.com

[R58] 下载文件
来源：http://reo.iojbl.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qwq.fengsongda.top

[R59] 发 POST JSON
来源：http://irj.tanke756.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wjs.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://npr.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ncr.daxiang520.top

[R61] 磁盘占用
来源：http://iec.bjfxy.top

df -h;  du -sh *
来源：http://dnz.smart0.xyz

[R62] 找最占空间的文件
来源：http://dul.jinqigufen.top

du -ah . | sort -rh | head -10
来源：http://wkv.cheryme.top

[R63] 内存与进程
来源：http://wrc.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://lyr.hnqzz.top

[R64] 结束进程
来源：http://byg.havefunace.top

kill -9 $(pgrep -f app.py)
来源：http://fki.epnwcf.com

[R65] 查看端口占用
来源：http://hrt.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ele.yvedp.cn

[R66] 定时任务
来源：http://xlr.fzhhl.top

crontab -e;  crontab -l
来源：http://gwf.birdmap.top

[R67] 生成随机十六进制串
来源：http://jia.c1oappe.top

openssl rand -hex 16
来源：http://stl.gzhubu.top

[R68] 计算文件校验值
来源：http://yee.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://bfj.yuxming.cn

[R69] 生成随机密码
来源：http://ewe.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://lmh.tianlin.xyz

[R70] 时间戳与互转
来源：http://wfp.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://suo.guannengcc.top

[R71] 日期格式化
来源：http://exa.hysaishi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yla.tarul.cn

[R72] 等待端口就绪
来源：http://nki.cucudq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vih.meibo888.top

[R73] 分割大日志
来源：http://jxk.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://hqq.sjlbkw.cn

[R74] 批量重命名
来源：http://cig.cheryme.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ecp.hnxiangtu.top

[R75] 导出环境变量
来源：http://ils.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://fmr.hfpthk.cn

[R76] 使用临时文件
来源：http://mbr.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gfc.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://yla.nwbrower.top

read -rp "请输入: " ans
来源：http://ozv.sjlbkw.cn

[R78] 交互式菜单
来源：http://coi.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://own.tanke756.top

[R79] 解析命令行选项
来源：http://rsk.cqqwz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oic.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://wrh.yongpay.top

time ./run.sh
来源：http://xkt.sufxvd.cn

================================================================================
来源：http://ful.zhoulong.xyz

S. C / C++ 专题
来源：http://jtf.zhoulong.xyz

================================================================================
来源：http://awd.316326.xyz

[S01] C：Hello World
来源：http://bjh.zdqjudy.top

#include <stdio.h>
来源：http://kuo.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://fdr.tian-w.cn

[S02] C：变量与格式化输出
来源：http://kdn.9152youxi.cn

int a = 10; printf("%d\n", a);
来源：http://nne.jinqigfzy.top

[S03] C：读入整数
来源：http://qoi.nwbrower.top

int x; scanf("%d", &x);
来源：http://oun.gzhubu.top

[S04] C：字符串复制
来源：http://tzg.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bob.c1oappe.top

[S05] C：字符串长度
来源：http://mjd.sysykeji.top

strlen(s)
来源：http://zur.gzhubu.top

[S06] C：字符串比较
来源：http://dlt.zhongyouzk.top

strcmp(a, b) == 0
来源：http://skv.sweek.top

[S07] C：数组遍历求和
来源：http://zjg.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jlj.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://olb.andypj.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eeq.fktsv.cn

[S09] C：结构体定义与初始化
来源：http://nrx.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mgj.xinyue.icu

[S10] C：指针与解引用
来源：http://kgp.iojbl.cn

int *p = &a;  *p = 5;
来源：http://iot.yuanzhike.top

[S11] C：逐行读文件
来源：http://ufh.zhixingplan.top

FILE *f = fopen("a.txt", "r");
来源：http://gih.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ier.hcnkem.com

fclose(f);
来源：http://wdy.gogol.net.cn

[S12] C：写文件
来源：http://toy.zdbjq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kbb.hnqzz.top

[S13] C：宏定义
来源：http://xik.jinyuanbaomall.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qct.ydzc1.top

[S14] C：枚举
来源：http://kav.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://wcp.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://pfw.chenjidiqi.icu

(double) a / b
来源：http://xnd.hysaishi.cn

[S16] C：位操作置位
来源：http://kob.zycfv.cn

x |= (1 << 3);
来源：http://bgq.cashguo.top

[S17] C：安全拼接字符串
来源：http://ezp.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zxg.guannengcc.top

[S18] C：命令行参数
来源：http://ggp.wangdashe.top

int main(int argc, char **argv)
来源：http://nmj.tarul.cn

[S19] C：快速排序
来源：http://tkq.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://mje.tianlin.xyz

[S20] C：二分查找
来源：http://yep.daria6918.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vyo.ehwqpu.com

[S21] C：字符类别判断
来源：http://tyg.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dca.tanke756.top

[S22] C：字符串转数字
来源：http://frj.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://iuf.zdbjq.cn

[S23] C：随机数
来源：http://flk.mhx1999.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uwj.sjlbkw.cn

[S24] C：获取本地时间
来源：http://cjo.sweek.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eey.daxiang520.top

[S25] C：内存拷贝
来源：http://qdx.cdnleiting.top

memcpy(dst, src, n);
来源：http://sfz.chenlongwang.top

[S26] C：内存清零
来源：http://ohb.jiagoushi.top

memset(a, 0, sizeof a);
来源：http://bnj.jqgfzy.top

[S27] C：定义常量
来源：http://ppg.gzhubu.top

const double PI = 3.14159;
来源：http://yzo.shuidangran.top

[S28] C：静态变量
来源：http://fnh.sjlbkw.cn

static int counter = 0;
来源：http://tui.gzhubu.top

[S29] C：变参函数
来源：http://juj.wangdashe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lzo.zhiwuduotai.top

[S30] C：头文件保护
来源：http://jsx.ivvv.top

#ifndef X_H
来源：http://zge.nwbrower.top

#define X_H
来源：http://piu.wangdashe.top

#endif
来源：http://sdc.chenzaomai.com

[S31] C++：Hello World
来源：http://fro.sxryk.cn

#include <iostream>
来源：http://ofm.snrcjt.cn

int main() { std::cout << "Hello\n"; }
来源：http://cyl.dianchejie.cn

[S32] C++：字符串
来源：http://vzt.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://rje.yongpay.top

[S33] C++：vector 增删
来源：http://hgy.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uqm.52xcode.cn

[S34] C++：遍历 vector
来源：http://xqn.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://efq.hfpthk.cn

[S35] C++：map
来源：http://zpx.yj20258.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uah.birdmap.top

[S36] C++：unordered_map
来源：http://jrm.sysykeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lly.zhoulong.xyz

[S37] C++：set
来源：http://wjd.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eht.zdbjq.cn

[S38] C++：排序
来源：http://ran.vqdsnc.cn

std::sort(v.begin(), v.end());
来源：http://ora.daria6918.cn


<!-- 参考信息 -->