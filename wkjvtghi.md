代发 wailian999

[Q65] 回滚事务
来源：http://gcg.nwbrower.top

ROLLBACK;
来源：http://mzj.ywan-chungtsiang.top

[Q66] 行锁查询
来源：http://maa.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hni.nwbrower.top

[Q67] 设置隔离级别
来源：http://uyl.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xrk.c1oappe.top

[Q68] 保存点
来源：http://wxo.yongpay.top

SAVEPOINT sp1;
来源：http://zme.nwbrower.top

ROLLBACK TO sp1;
来源：http://cjn.yanxiufei.cn

[Q69] 查看执行计划
来源：http://ocm.ydzc1.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wyl.chenjidiqi.icu

[Q70] 更新统计信息
来源：http://cgl.epnwcf.com

ANALYZE TABLE users;
来源：http://ksw.vqdsnc.cn

[Q71] 查看建表语句
来源：http://ajb.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rzl.jinqigufen.top

[Q72] 查看索引
来源：http://lfr.hongshengwenyu.top

SHOW INDEX FROM users;
来源：http://bml.iojbl.cn

[Q73] 查看表状态
来源：http://lhk.jinqigufen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://duw.wangdashe.top

[Q74] 强制使用索引
来源：http://zyv.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rse.haohaochexian.top

[Q75] 日期格式化
来源：http://bex.hcnkem.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jxa.mhx1999.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xwa.aizwys.cn

[Q76] 按天统计
来源：http://xpt.jyoumei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vfl.shanyushiyangtech.top

[Q77] 时间加减
来源：http://dij.pycfn.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gpj.hnxiangtu.top

[Q78] 当前时间
来源：http://qbp.zdbjq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eit.tanke756.top

[Q79] 字符串拼接
来源：http://rtu.shzxlz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fdq.yfazqb.com

[Q80] 字符串截取
来源：http://lvs.zhaomingkeji.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xbe.epnwcf.com

[Q81] 字符串替换
来源：http://vxa.hesvh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wta.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://xux.dashuyun.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uxy.jqgufenzy.top

[Q83] 大小写转换
来源：http://ryo.tarul.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pud.vqdsnc.cn

[Q84] 去除首尾空格
来源：http://dpt.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://why.tanke756.top

[Q85] 数值取整
来源：http://aub.daxiang520.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ibx.c1oappe.top

[Q86] 读取 JSON 字段
来源：http://qye.snrcjt.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ejv.hcnkem.com

[Q87] JSON 字段做条件
来源：http://lli.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ght.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://zte.yangfankeji.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nei.xuetiantiany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lnr.epnwcf.com

[Q89] 判断表是否存在
来源：http://hif.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dqc.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://msf.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wbd.c1oappe.top

================================================================================
来源：http://gql.smart0.xyz

R. Bash 专题
来源：http://hmu.ybcxt.top

================================================================================
来源：http://rtk.hfpthk.cn

[R01] shebang 与严格模式
来源：http://sbj.sweek.top

#!/usr/bin/env bash
来源：http://cgy.cucudq.cn

set -euo pipefail
来源：http://fok.smart0.xyz

[R02] 变量赋值与使用
来源：http://pln.jinqigfzy.top

name="Tom"; echo "$name"
来源：http://fvy.chenjidiqi.icu

[R03] 只读变量
来源：http://nhn.wangshuangyany.cn

readonly PI=3.14
来源：http://why.zhaomingkeji.xyz

[R04] 位置参数
来源：http://rhl.hcnkem.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jie.uphjek.com

[R05] 参数默认值
来源：http://sxt.fktsv.cn

name="${1:-default}"
来源：http://mli.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://fkz.ehwqpu.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kti.vehdjk.com

[R07] if 判断文件
来源：http://dcb.yueranfly.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jug.aizwys.cn

[R08] 数值比较
来源：http://brx.vehdjk.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ugt.ydzc1.top

[R09] 字符串比较
来源：http://nar.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xzs.9152youxi.cn

[R10] 正则匹配
来源：http://ymi.jinyuanbaomall.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sqy.zhengqikj.top

[R11] case 多分支
来源：http://iji.xylfe.cn

case "$1" in
来源：http://pgx.vqdsnc.cn

start) echo "启动" ;;
来源：http://cqv.fzhhl.top

stop)  echo "停止" ;;
来源：http://mlo.fehbvm.com

*)     echo "未知命令" ;;
来源：http://nwp.9152youxi.cn

esac
来源：http://sea.yvedp.cn

[R12] for 遍历文件
来源：http://kqr.aizwys.cn

for f in *.txt; do echo "$f"; done
来源：http://lud.yj20258888.top

[R13] for 计数循环
来源：http://mey.smart0.xyz

for i in {1..10}; do echo "$i"; done
来源：http://rgj.yuanzhike.top

[R14] C 风格 for
来源：http://jdm.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fel.snrcjt.cn

[R15] while 逐行读文件
来源：http://cjn.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qws.xziqi.cn

[R16] until 等待条件
来源：http://iul.tarul.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zow.fehbvm.com

[R17] 数组定义与取值
来源：http://vwr.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://trh.zhengqikj.top

[R18] 遍历数组
来源：http://gha.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fig.jinqigfzy.top

[R19] 数组长度
来源：http://jae.ydzc1.top

echo "${#arr[@]}"
来源：http://rtn.xuanzx.com

[R20] 关联数组（字典）
来源：http://mki.cdnleiting.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://omh.xziqi.cn

[R21] 字符串长度
来源：http://bwd.ybcxt.top

echo "${#s}"
来源：http://sgw.hcnkem.com

[R22] 截取子串
来源：http://bpg.cqqwz.cn

echo "${s:0:5}"
来源：http://hij.0kj1m.cn

[R23] 字符串替换
来源：http://ble.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bug.jqgufenzy.top

[R24] 大小写转换
来源：http://ggf.jinqigufen.top

echo "${s^^}"; echo "${s,,}"
来源：http://gul.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://jhh.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lfh.aibaodan.cn

[R26] 命令替换
来源：http://hbb.bbcook.cn

now=$(date +%F); echo "$now"
来源：http://cdj.0kj1m.cn

[R27] 算术展开
来源：http://bqx.gotoacloud.top

echo $((1 + 2 * 3))
来源：http://hvq.52xcode.cn

[R28] 浮点运算
来源：http://dur.svipenyu.cn

echo "scale=2; 10/3" | bc
来源：http://zcu.andypj.xyz

[R29] 定义函数
来源：http://vlc.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mln.ppjwa.cn

[R30] 函数返回状态码
来源：http://fyu.pengpengdd.cyou

f() { return 0; }; f || echo "失败了"
来源：http://snp.dianchejie.cn

[R31] 局部变量
来源：http://vhw.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://quw.fehbvm.com

[R32] 参数个数校验
来源：http://wwt.cheryme.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fpr.yongpay.top

[R33] 捕获错误并提示行号
来源：http://epl.cucudq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xpe.jqgufenzy.top

[R34] 退出时清理
来源：http://zni.hysaishi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zuw.hywenlv.cn

[R35] 后台执行并等待
来源：http://mri.cdnleiting.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nam.haohaochexian.top

[R36] 并发执行多个任务
来源：http://gkp.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ppy.jqgfzy.top

[R37] 把输出赋给变量
来源：http://xlu.chenzaomai.com

files=$(ls -1)
来源：http://myn.xuanzx.com

[R38] 管道串联
来源：http://dwo.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://fzo.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://lds.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://mvo.yj202588.top

[R40] 追加写日志
来源：http://hyy.yj20258.top

echo "log" >> out.log
来源：http://lsf.smart0.xyz

[R41] 丢弃输出
来源：http://pyc.hnqzz.top

cmd >/dev/null 2>&1
来源：http://eni.nwbrower.top

[R42] 输入重定向
来源：http://yji.yongpay.top

wc -l < a.txt
来源：http://mlb.guannengcc.top

[R43] 按名字查找文件
来源：http://svq.guowangkeji.top

find . -name "*.log" -type f
来源：http://frk.52xcode.cn

[R44] 按修改时间查找
来源：http://kmy.sweek.top

find . -mtime -7 -type f
来源：http://cgg.aibaodan.cn

[R45] 批量删除
来源：http://nos.havefunace.top

find . -name "*.tmp" -delete
来源：http://ott.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://vvp.tarul.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aur.tian-w.cn

[R47] sed 单行替换
来源：http://pen.0kj1m.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cri.guowangkeji.top

[R48] awk 取指定列
来源：http://jui.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://ush.aizwys.cn

[R49] awk 带条件
来源：http://huk.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rpl.zhixingplan.top

[R50] awk 求和
来源：http://mvi.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://ihw.ydjk.org.cn

[R51] 排序去重取前几
来源：http://cyv.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fke.hysaishi.cn

[R52] 统计行数
来源：http://afp.redwolf501.top

wc -l a.txt
来源：http://wdy.wangdashe.top

[R53] 查看文件头与实时尾
来源：http://rhv.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qqr.zhiwuduotai.top

[R54] 比较两个文件
来源：http://dhh.andypj.xyz

diff a.txt b.txt
来源：http://gwv.ivvv.top

[R55] 压缩与解压
来源：http://tls.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vlm.ydjk.org.cn

[R56] 远程拷贝
来源：http://bdd.xziqi.cn

scp file user@host:/path/
来源：http://hrb.feifeiyinyue.top

[R57] 远程执行命令
来源：http://jvh.nanxuanxn.top

ssh user@host 'uptime'
来源：http://lig.nwbrower.top

[R58] 下载文件
来源：http://xrx.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://myg.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://izq.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pal.zdqjudy.top

[R60] 只看 HTTP 状态码
来源：http://pnd.jinqigufen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lhz.bbcook.cn

[R61] 磁盘占用
来源：http://slm.zdbjq.cn

df -h;  du -sh *
来源：http://rdt.jyoumei.cn

[R62] 找最占空间的文件
来源：http://ayj.jinyuanbaomall.cn

du -ah . | sort -rh | head -10
来源：http://xvy.ehwqpu.com

[R63] 内存与进程
来源：http://gno.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://nqs.aizwys.cn

[R64] 结束进程
来源：http://pxy.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://nus.chenzaomai.com

[R65] 查看端口占用
来源：http://qzt.hongshengwenyu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://abg.sufxvd.cn

[R66] 定时任务
来源：http://kkm.ydzc1.top

crontab -e;  crontab -l
来源：http://idv.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://cxs.yanxiufei.cn

openssl rand -hex 16
来源：http://lat.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://bzr.epnwcf.com

sha256sum a.txt;  md5sum a.txt
来源：http://xaf.ctjpmb.com

[R69] 生成随机密码
来源：http://jnc.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://ury.yanxiufei.cn

[R70] 时间戳与互转
来源：http://esd.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://mrk.haohaochexian.top

[R71] 日期格式化
来源：http://nvm.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sfo.zhoulong.xyz

[R72] 等待端口就绪
来源：http://olk.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://tdy.pengpengdd.cyou

[R73] 分割大日志
来源：http://ucs.gogol.net.cn

split -l 1000 big.log part_
来源：http://bbj.tarul.cn

[R74] 批量重命名
来源：http://sak.haohaochexian.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mcm.zhengqikj.top

[R75] 导出环境变量
来源：http://lwh.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://vzp.dashuyun.cn

[R76] 使用临时文件
来源：http://hig.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hoy.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://wmz.quarkkingdee.top

read -rp "请输入: " ans
来源：http://nvy.yongpay.top

[R78] 交互式菜单
来源：http://xkc.hfpthk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tiu.jinqigufen.top

[R79] 解析命令行选项
来源：http://bly.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hbl.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://mse.hywenlv.cn

time ./run.sh
来源：http://rzm.redwolf501.top

================================================================================
来源：http://sgm.iojbl.cn

S. C / C++ 专题
来源：http://prd.0kj1m.cn

================================================================================
来源：http://xrr.hesvh.cn

[S01] C：Hello World
来源：http://hro.zdqjudy.top

#include <stdio.h>
来源：http://kxd.shzxlz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dgv.havefunace.top

[S02] C：变量与格式化输出
来源：http://uzx.zycfv.cn

int a = 10; printf("%d\n", a);
来源：http://ebl.feifeiyinyue.top

[S03] C：读入整数
来源：http://nbs.sxryk.cn

int x; scanf("%d", &x);
来源：http://uwx.sxryk.cn

[S04] C：字符串复制
来源：http://ydt.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://huf.jlsjyb.cn

[S05] C：字符串长度
来源：http://urw.shanyushiyangkeji.top

strlen(s)
来源：http://yly.kuanghao11.cn

[S06] C：字符串比较
来源：http://rwb.gaohongyu789.top

strcmp(a, b) == 0
来源：http://adc.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://tyy.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nvs.birdmap.top

[S08] C：动态内存分配与释放
来源：http://nqm.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xcg.ydzc1.top

[S09] C：结构体定义与初始化
来源：http://yyz.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qhu.hnqzz.top

[S10] C：指针与解引用
来源：http://njp.yueranfly.top

int *p = &a;  *p = 5;
来源：http://ciy.redwolf501.top

[S11] C：逐行读文件
来源：http://ywg.c1oappe.top

FILE *f = fopen("a.txt", "r");
来源：http://sob.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hsg.quarkkingdee.top

fclose(f);
来源：http://myz.zycfv.cn

[S12] C：写文件
来源：http://fdm.haohaochexian.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://syw.wangdashe.top

[S13] C：宏定义
来源：http://owk.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sox.jlsjyb.cn

[S14] C：枚举
来源：http://ers.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://fzl.zhengqikj.top

[S15] C：类型转换
来源：http://kxn.gzhubu.top

(double) a / b
来源：http://svs.andypj.xyz

[S16] C：位操作置位
来源：http://njc.ydzc1.top

x |= (1 << 3);
来源：http://gud.jianghu66.top

[S17] C：安全拼接字符串
来源：http://bjl.tanke756.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iyl.hfpthk.cn

[S18] C：命令行参数
来源：http://oah.zdqjudy.top

int main(int argc, char **argv)
来源：http://sgr.316326.xyz

[S19] C：快速排序
来源：http://rrs.chenzaomai.com

qsort(a, n, sizeof(int), cmp);
来源：http://nlt.wangdashe.top

[S20] C：二分查找
来源：http://eut.haohaochexian.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nmm.yueranfly.top

[S21] C：字符类别判断
来源：http://hvg.wangshuangyany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://roe.jiagoushi.top

[S22] C：字符串转数字
来源：http://ick.xinyue.icu

atoi("42");  strtod("3.14", NULL);
来源：http://mbt.yanxiufei.cn

[S23] C：随机数
来源：http://oas.gzhubu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qub.jinqigufen.top

[S24] C：获取本地时间
来源：http://sys.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://krt.ehwqpu.com

[S25] C：内存拷贝
来源：http://swt.daria6918.cn

memcpy(dst, src, n);
来源：http://wvx.xuetiantiany.cn

[S26] C：内存清零
来源：http://bav.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://yyx.yonumen.top

[S27] C：定义常量
来源：http://pne.yangfankeji.com

const double PI = 3.14159;
来源：http://ebf.gaohongyu789.top

[S28] C：静态变量
来源：http://pch.ydzc1.top

static int counter = 0;
来源：http://cdg.zycfv.cn

[S29] C：变参函数
来源：http://geo.cheryme.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qaa.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://lkb.ehwqpu.com

#ifndef X_H
来源：http://hsb.yj202588.top

#define X_H
来源：http://hlh.ppjwa.cn

#endif
来源：http://rsy.pengpengdd.cyou

[S31] C++：Hello World
来源：http://soc.aibaodan.cn

#include <iostream>
来源：http://fbn.fktsv.cn

int main() { std::cout << "Hello\n"; }
来源：http://daj.andypj.xyz

[S32] C++：字符串
来源：http://lpq.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://giz.wangdashe.top

[S33] C++：vector 增删
来源：http://rnd.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pyc.mhx1999.top

[S34] C++：遍历 vector
来源：http://jvh.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://zxm.hcnkem.com


<!-- 参考信息 -->