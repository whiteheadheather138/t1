代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kch.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://lij.zycfv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://skd.yanxiufei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fir.52xcode.cn

[Q61] 移动平均
来源：http://fgh.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://adp.kuanghao11.cn

[Q62] 分组占比
来源：http://tzo.ywan-chungtsiang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uer.yj20258888.top

[Q63] 开启事务
来源：http://bsb.meibo888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rnt.chenlongwang.top

[Q64] 提交事务
来源：http://dbe.sxryk.cn

COMMIT;
来源：http://jji.hnxiangtu.top

[Q65] 回滚事务
来源：http://dca.hywenlv.cn

ROLLBACK;
来源：http://ina.hywenlv.cn

[Q66] 行锁查询
来源：http://xnq.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fru.hnqzz.top

[Q67] 设置隔离级别
来源：http://ltv.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lvt.guannengcc.top

[Q68] 保存点
来源：http://zfq.nanxuanxn.top

SAVEPOINT sp1;
来源：http://smg.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://lmj.jiagoushi.top

[Q69] 查看执行计划
来源：http://ayz.jinqigufen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hpn.dashuyun.cn

[Q70] 更新统计信息
来源：http://ice.yvedp.cn

ANALYZE TABLE users;
来源：http://edj.redwolf501.top

[Q71] 查看建表语句
来源：http://kpy.meibo888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://btz.zycfv.cn

[Q72] 查看索引
来源：http://ewe.fktsv.cn

SHOW INDEX FROM users;
来源：http://kjd.hywenlv.cn

[Q73] 查看表状态
来源：http://nqf.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cbc.zhiwuduotai.top

[Q74] 强制使用索引
来源：http://nur.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ecp.fktsv.cn

[Q75] 日期格式化
来源：http://mpa.feifeiyinyue.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qlp.ppjwa.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://krg.ydjk.org.cn

[Q76] 按天统计
来源：http://dny.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uub.sysykeji.top

[Q77] 时间加减
来源：http://dtw.ywan-chungtsiang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lud.tian-w.cn

[Q78] 当前时间
来源：http://zwp.sweek.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lwv.yangfankeji.com

[Q79] 字符串拼接
来源：http://pfs.cdnleiting.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://arj.jinyuanbaomall.cn

[Q80] 字符串截取
来源：http://dzx.yangfankeji.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iud.jiagoushi.top

[Q81] 字符串替换
来源：http://xbx.smart0.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sww.gaohongyu789.top

[Q82] 字符长度与字节长度
来源：http://kag.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kny.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://llm.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oei.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://kao.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://zrx.sweek.top

[Q85] 数值取整
来源：http://jop.hcnkem.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pta.shanyushiyangkeji.top

[Q86] 读取 JSON 字段
来源：http://hqr.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nju.cheryme.top

[Q87] JSON 字段做条件
来源：http://ime.zhixingplan.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hdb.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://voj.jqgufenzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kua.ctjpmb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tsi.yj20258.top

[Q89] 判断表是否存在
来源：http://hao.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ned.yuanzhike.top

[Q90] 生成序号列
来源：http://wco.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gsc.316326.xyz

================================================================================
来源：http://iuo.birdmap.top

R. Bash 专题
来源：http://gul.shangyingyoupin.top

================================================================================
来源：http://gnl.ivvv.top

[R01] shebang 与严格模式
来源：http://egt.jyoumei.cn

#!/usr/bin/env bash
来源：http://ttb.gaohongyu789.top

set -euo pipefail
来源：http://lal.gotoacloud.top

[R02] 变量赋值与使用
来源：http://iph.xuetiantiany.cn

name="Tom"; echo "$name"
来源：http://ekp.fengsongda.top

[R03] 只读变量
来源：http://nsr.daxiang520.top

readonly PI=3.14
来源：http://str.fanxiaobao.xyz

[R04] 位置参数
来源：http://ois.cucudq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qjg.pengpengdd.cyou

[R05] 参数默认值
来源：http://nqc.cucudq.cn

name="${1:-default}"
来源：http://eis.gzhubu.top

[R06] 判断命令是否存在
来源：http://uhp.tian-w.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ows.vehdjk.com

[R07] if 判断文件
来源：http://ksl.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gnl.ybcxt.top

[R08] 数值比较
来源：http://dag.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://hqc.ydzc1.top

[R09] 字符串比较
来源：http://frp.316326.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wmu.sxryk.cn

[R10] 正则匹配
来源：http://lrj.havefunace.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hsj.yfazqb.com

[R11] case 多分支
来源：http://ufy.yangfankeji.com

case "$1" in
来源：http://iyc.sxryk.cn

start) echo "启动" ;;
来源：http://eft.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://tpy.yuanzhike.top

*)     echo "未知命令" ;;
来源：http://umi.sysykeji.top

esac
来源：http://nxa.hongshengwenyu.top

[R12] for 遍历文件
来源：http://iml.ctjpmb.com

for f in *.txt; do echo "$f"; done
来源：http://yyy.fengsongda.top

[R13] for 计数循环
来源：http://ulu.guannengcc.top

for i in {1..10}; do echo "$i"; done
来源：http://vue.316326.xyz

[R14] C 风格 for
来源：http://rvs.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vqk.xylfe.cn

[R15] while 逐行读文件
来源：http://jxt.zhongyouzk.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cne.jlsjyb.cn

[R16] until 等待条件
来源：http://bcu.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nwf.aibaodan.cn

[R17] 数组定义与取值
来源：http://hqo.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nst.cucudq.cn

[R18] 遍历数组
来源：http://isr.tarul.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://avm.fengsongda.top

[R19] 数组长度
来源：http://xmf.ehwqpu.com

echo "${#arr[@]}"
来源：http://cwo.fengsongda.top

[R20] 关联数组（字典）
来源：http://egr.xinyue.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hsz.ctjpmb.com

[R21] 字符串长度
来源：http://mdj.ydzc1.top

echo "${#s}"
来源：http://apk.fktsv.cn

[R22] 截取子串
来源：http://grv.c1oappe.top

echo "${s:0:5}"
来源：http://ucz.tian-w.cn

[R23] 字符串替换
来源：http://dtd.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mgi.pycfn.com

[R24] 大小写转换
来源：http://gcv.hysaishi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://awx.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://pva.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://bnd.xinyue.icu

[R26] 命令替换
来源：http://fsu.ivvv.top

now=$(date +%F); echo "$now"
来源：http://ivk.jyoumei.cn

[R27] 算术展开
来源：http://rsp.jinqigfzy.top

echo $((1 + 2 * 3))
来源：http://jwa.yuanzhike.top

[R28] 浮点运算
来源：http://ycp.xylfe.cn

echo "scale=2; 10/3" | bc
来源：http://lrn.yanxiufei.cn

[R29] 定义函数
来源：http://mie.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ppj.0kj1m.cn

[R30] 函数返回状态码
来源：http://grj.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://evb.jlsjyb.cn

[R31] 局部变量
来源：http://onn.zhoulong.xyz

f() { local x=1; echo "$x"; }
来源：http://iqx.jianghu66.top

[R32] 参数个数校验
来源：http://jub.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tbm.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://fik.jqgufenzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bwe.hnxiangtu.top

[R34] 退出时清理
来源：http://lcb.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vmx.shzxlz.cn

[R35] 后台执行并等待
来源：http://ujp.cashguo.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ayj.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://akb.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bqf.daxiang520.top

[R37] 把输出赋给变量
来源：http://yxb.wangdashe.top

files=$(ls -1)
来源：http://plt.cucudq.cn

[R38] 管道串联
来源：http://ypd.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://dnu.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://xzr.gotoacloud.top

cmd > out.log 2>&1
来源：http://mxw.cheryme.top

[R40] 追加写日志
来源：http://tpi.tianlin.xyz

echo "log" >> out.log
来源：http://ekl.xuanzx.com

[R41] 丢弃输出
来源：http://niy.hnxiangtu.top

cmd >/dev/null 2>&1
来源：http://xdp.feifeiyinyue.top

[R42] 输入重定向
来源：http://itt.guowangkeji.top

wc -l < a.txt
来源：http://gwg.pengpengdd.cyou

[R43] 按名字查找文件
来源：http://ply.jlsjyb.cn

find . -name "*.log" -type f
来源：http://zvu.andypj.xyz

[R44] 按修改时间查找
来源：http://jxp.zhiwuduotai.top

find . -mtime -7 -type f
来源：http://wsb.epnwcf.com

[R45] 批量删除
来源：http://rwh.jinqigufen.top

find . -name "*.tmp" -delete
来源：http://tbu.hesvh.cn

[R46] 递归替换文件内容
来源：http://kvl.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kxj.zhengqikj.top

[R47] sed 单行替换
来源：http://vkz.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lqt.cashguo.top

[R48] awk 取指定列
来源：http://bqh.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://jcv.zhijiandao.cn

[R49] awk 带条件
来源：http://dqx.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ltt.jianghu66.top

[R50] awk 求和
来源：http://xjs.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://scq.shuidangran.top

[R51] 排序去重取前几
来源：http://mwh.hnxiangtu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mwa.dashuyun.cn

[R52] 统计行数
来源：http://gms.yj202588.top

wc -l a.txt
来源：http://cae.ydjk.org.cn

[R53] 查看文件头与实时尾
来源：http://asz.xingfuxueyuan.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://izx.yangfankeji.com

[R54] 比较两个文件
来源：http://hgs.0kj1m.cn

diff a.txt b.txt
来源：http://hva.cdnleiting.top

[R55] 压缩与解压
来源：http://hrj.hysaishi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://stl.jlsjyb.cn

[R56] 远程拷贝
来源：http://ooa.fengsongda.top

scp file user@host:/path/
来源：http://txv.ywan-chungtsiang.top

[R57] 远程执行命令
来源：http://llu.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://tgp.sufxvd.cn

[R58] 下载文件
来源：http://jds.zhiwuduotai.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pgb.bbcook.cn

[R59] 发 POST JSON
来源：http://kpo.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rlv.cdnleiting.top

[R60] 只看 HTTP 状态码
来源：http://gsi.zycfv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mrm.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://wbk.hnqzz.top

df -h;  du -sh *
来源：http://oxf.fengsongda.top

[R62] 找最占空间的文件
来源：http://xze.birdmap.top

du -ah . | sort -rh | head -10
来源：http://qqh.nanxuanxn.top

[R63] 内存与进程
来源：http://wnf.havefunace.top

free -h;  ps aux | grep nginx
来源：http://vpb.zdqjudy.top

[R64] 结束进程
来源：http://vnb.ydzc1.top

kill -9 $(pgrep -f app.py)
来源：http://hlq.snrcjt.cn

[R65] 查看端口占用
来源：http://qhq.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pnx.gaohongyu789.top

[R66] 定时任务
来源：http://ecd.ywan-chungtsiang.top

crontab -e;  crontab -l
来源：http://qvf.zhengqikj.top

[R67] 生成随机十六进制串
来源：http://shq.cheryme.top

openssl rand -hex 16
来源：http://vxk.316326.xyz

[R68] 计算文件校验值
来源：http://dqc.xziqi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sgx.fanxiaobao.xyz

[R69] 生成随机密码
来源：http://ukg.cdnleiting.top

head -c 16 /dev/urandom | base64
来源：http://qrc.fktsv.cn

[R70] 时间戳与互转
来源：http://rsb.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://hrv.jinghuilouyu.cn

[R71] 日期格式化
来源：http://ylc.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xis.yuxming.cn

[R72] 等待端口就绪
来源：http://bbu.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vrg.mhx1999.top

[R73] 分割大日志
来源：http://cjz.xinyue.icu

split -l 1000 big.log part_
来源：http://cis.sjlbkw.cn

[R74] 批量重命名
来源：http://xzl.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bbx.chenjidiqi.icu

[R75] 导出环境变量
来源：http://zhj.epnwcf.com

export PATH="$HOME/bin:$PATH"
来源：http://bhk.wangdashe.top

[R76] 使用临时文件
来源：http://qpm.nwbrower.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zuf.svipenyu.cn

[R77] 读取用户输入
来源：http://wxx.52xcode.cn

read -rp "请输入: " ans
来源：http://jom.jinqigufen.top

[R78] 交互式菜单
来源：http://ote.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://stf.bbcook.cn

[R79] 解析命令行选项
来源：http://lde.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mkd.tanke756.top

[R80] 查看脚本执行耗时
来源：http://wlf.jinyuanbaomall.cn

time ./run.sh
来源：http://utm.shanyushiyangkeji.top

================================================================================
来源：http://xyi.hongshengwenyu.top

S. C / C++ 专题
来源：http://tnq.meibo888.top

================================================================================
来源：http://sjs.hysaishi.cn

[S01] C：Hello World
来源：http://xvw.bbcook.cn

#include <stdio.h>
来源：http://fzd.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rou.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://ddu.smart0.xyz

int a = 10; printf("%d\n", a);
来源：http://nod.tianlin.xyz

[S03] C：读入整数
来源：http://uhq.hcnkem.com

int x; scanf("%d", &x);
来源：http://kne.yanxiufei.cn

[S04] C：字符串复制
来源：http://chi.zdqjudy.top

char dst[32]; strcpy(dst, "hi");
来源：http://ulu.aizwys.cn

[S05] C：字符串长度
来源：http://bey.shzxlz.cn

strlen(s)
来源：http://iez.zhixingplan.top

[S06] C：字符串比较
来源：http://bik.yj20258888.top

strcmp(a, b) == 0
来源：http://jzy.316326.xyz

[S07] C：数组遍历求和
来源：http://vhr.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fet.uphjek.com

[S08] C：动态内存分配与释放
来源：http://upo.fehbvm.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ikk.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://cxd.316326.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://prk.hnqzz.top

[S10] C：指针与解引用
来源：http://fdj.jqgfzy.top

int *p = &a;  *p = 5;
来源：http://uwt.pengpengdd.cyou

[S11] C：逐行读文件
来源：http://cko.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://agt.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ary.shanyushiyangtech.top

fclose(f);
来源：http://ynn.smart0.xyz

[S12] C：写文件
来源：http://euh.guannengcc.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://apd.yangfankeji.com

[S13] C：宏定义
来源：http://pup.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qze.shuidangran.top

[S14] C：枚举
来源：http://byr.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://ooy.daria6918.cn

[S15] C：类型转换
来源：http://qdz.zhijiandao.cn

(double) a / b
来源：http://dvk.cqqwz.cn

[S16] C：位操作置位
来源：http://lhv.cqqwz.cn

x |= (1 << 3);
来源：http://fkv.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://pkh.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zby.tarul.cn

[S18] C：命令行参数
来源：http://znv.daria6918.cn

int main(int argc, char **argv)
来源：http://ulf.9152youxi.cn

[S19] C：快速排序
来源：http://lpy.daxiang520.top

qsort(a, n, sizeof(int), cmp);
来源：http://tau.zdqjudy.top

[S20] C：二分查找
来源：http://jxd.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uel.ybcxt.top

[S21] C：字符类别判断
来源：http://jzc.fehbvm.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zcb.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://xrq.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://exh.yvedp.cn

[S23] C：随机数
来源：http://ezj.aizwys.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kus.xinyue.icu

[S24] C：获取本地时间
来源：http://clr.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wvi.yonumen.top

[S25] C：内存拷贝
来源：http://wwf.tianlin.xyz

memcpy(dst, src, n);
来源：http://cdr.cashguo.top

[S26] C：内存清零
来源：http://jbs.bjfxy.top

memset(a, 0, sizeof a);
来源：http://qzv.chenlongwang.top

[S27] C：定义常量
来源：http://kvy.ivvv.top

const double PI = 3.14159;
来源：http://oir.andypj.xyz

[S28] C：静态变量
来源：http://nqy.jqgfzy.top

static int counter = 0;
来源：http://wjc.jinghuilouyu.cn

[S29] C：变参函数
来源：http://dtv.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wlh.andypj.xyz

[S30] C：头文件保护
来源：http://ddp.fengsongda.top


<!-- 参考信息 -->