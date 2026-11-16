代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://anl.xziqi.cn

[Q50] 批量更新
来源：http://vsv.xingfuxueyuan.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dvy.yvedp.cn

[Q51] 用子查询更新
来源：http://ift.yanxiufei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://otb.daxiang520.top

[Q52] 删除指定行
来源：http://enu.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://ttn.yj20258.top

[Q53] 按条件删除
来源：http://kfq.aizwys.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://krx.sjlbkw.cn

[Q54] 清空表
来源：http://mlh.guowangkeji.top

TRUNCATE TABLE logs;
来源：http://xll.sufxvd.cn

[Q55] 排名（并列占位）
来源：http://fiu.9152youxi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qeh.cucudq.cn

[Q56] 密集排名（并列不占位）
来源：http://kdd.xinyue.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gpd.hnxiangtu.top

[Q57] 行号
来源：http://frx.xinyue.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dcg.bjfxy.top

[Q58] 累计求和
来源：http://fwy.hammf.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yus.guowangkeji.top

[Q59] 分组内累计
来源：http://ofl.tanke756.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lbs.hysaishi.cn

[Q60] 取上一行 / 下一行
来源：http://amo.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ogw.zdbjq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://grr.chenjidiqi.icu

[Q61] 移动平均
来源：http://yyi.quarkkingdee.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dwj.gogol.net.cn

[Q62] 分组占比
来源：http://otk.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gpx.chenlongwang.top

[Q63] 开启事务
来源：http://vcv.jinyuanbaomall.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fcy.aizwys.cn

[Q64] 提交事务
来源：http://ikw.jyoumei.cn

COMMIT;
来源：http://dtx.hammf.cn

[Q65] 回滚事务
来源：http://epz.dianchejie.cn

ROLLBACK;
来源：http://cwa.hesvh.cn

[Q66] 行锁查询
来源：http://kmk.yj20258.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://alz.9152youxi.cn

[Q67] 设置隔离级别
来源：http://klb.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yhz.yuanzhike.top

[Q68] 保存点
来源：http://eyg.uphjek.com

SAVEPOINT sp1;
来源：http://nzc.aizwys.cn

ROLLBACK TO sp1;
来源：http://zaf.chenzaomai.com

[Q69] 查看执行计划
来源：http://mks.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hyt.gotoacloud.top

[Q70] 更新统计信息
来源：http://uut.yj202588.top

ANALYZE TABLE users;
来源：http://htq.epnwcf.com

[Q71] 查看建表语句
来源：http://hbw.hnqzz.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vmu.ydzc1.top

[Q72] 查看索引
来源：http://iit.yonumen.top

SHOW INDEX FROM users;
来源：http://vxt.andypj.xyz

[Q73] 查看表状态
来源：http://szi.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xag.jqgfzy.top

[Q74] 强制使用索引
来源：http://ewz.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blu.xziqi.cn

[Q75] 日期格式化
来源：http://jgs.dianchejie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ngc.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bxu.shangyingyoupin.top

[Q76] 按天统计
来源：http://wkl.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://deu.jinghuilouyu.cn

[Q77] 时间加减
来源：http://yml.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vuc.yueranfly.top

[Q78] 当前时间
来源：http://fdx.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kxx.zhixingplan.top

[Q79] 字符串拼接
来源：http://omm.jinqigufen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aar.yj202588.top

[Q80] 字符串截取
来源：http://fdd.aibaodan.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nyy.bbcook.cn

[Q81] 字符串替换
来源：http://prw.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rxp.vqdsnc.cn

[Q82] 字符长度与字节长度
来源：http://hdb.hcnkem.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://czk.wangshuangyany.cn

[Q83] 大小写转换
来源：http://hra.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ywa.daxiang520.top

[Q84] 去除首尾空格
来源：http://ygd.daria6918.cn

SELECT TRIM(name) FROM users;
来源：http://xfh.xziqi.cn

[Q85] 数值取整
来源：http://lfn.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ine.cqqwz.cn

[Q86] 读取 JSON 字段
来源：http://dkb.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ytr.jinqigufen.top

[Q87] JSON 字段做条件
来源：http://jpr.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nqr.fktsv.cn

[Q88] 行转列（条件聚合）
来源：http://ulz.yuxming.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vtl.cqqwz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ncx.aibaodan.cn

[Q89] 判断表是否存在
来源：http://ayu.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bww.yongpay.top

[Q90] 生成序号列
来源：http://gyr.tarul.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zmv.jinghuilouyu.cn

================================================================================
来源：http://qew.jianghu66.top

R. Bash 专题
来源：http://bun.xingfuxueyuan.xyz

================================================================================
来源：http://nsl.redwolf501.top

[R01] shebang 与严格模式
来源：http://fjk.epnwcf.com

#!/usr/bin/env bash
来源：http://qws.hfpthk.cn

set -euo pipefail
来源：http://zyd.xinyue.icu

[R02] 变量赋值与使用
来源：http://ocn.yj20258888.top

name="Tom"; echo "$name"
来源：http://wlx.tianlin.xyz

[R03] 只读变量
来源：http://rec.cucudq.cn

readonly PI=3.14
来源：http://wqk.meibo888.top

[R04] 位置参数
来源：http://kcd.shuidangran.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://weu.gogol.net.cn

[R05] 参数默认值
来源：http://aua.nanxinkj.top

name="${1:-default}"
来源：http://mfw.xuanzx.com

[R06] 判断命令是否存在
来源：http://ssv.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yyi.yfazqb.com

[R07] if 判断文件
来源：http://unl.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sng.zdqjudy.top

[R08] 数值比较
来源：http://srd.yj20258.top

if (( a > b )); then echo "a 更大"; fi
来源：http://die.vehdjk.com

[R09] 字符串比较
来源：http://sxn.zhixingplan.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ibv.quarkkingdee.top

[R10] 正则匹配
来源：http://kuz.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iml.vehdjk.com

[R11] case 多分支
来源：http://cvo.c1oappe.top

case "$1" in
来源：http://ucy.wangdashe.top

start) echo "启动" ;;
来源：http://hvd.sxryk.cn

stop)  echo "停止" ;;
来源：http://aeb.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://esf.316326.xyz

esac
来源：http://men.hnqzz.top

[R12] for 遍历文件
来源：http://gai.jqgufenzy.top

for f in *.txt; do echo "$f"; done
来源：http://cbm.ivvv.top

[R13] for 计数循环
来源：http://azz.hongshengwenyu.top

for i in {1..10}; do echo "$i"; done
来源：http://ysl.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://vky.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fyp.zhixingplan.top

[R15] while 逐行读文件
来源：http://jqh.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://itj.sjlbkw.cn

[R16] until 等待条件
来源：http://czd.tarul.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sdh.yuanzhike.top

[R17] 数组定义与取值
来源：http://hew.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fzk.ywan-chungtsiang.top

[R18] 遍历数组
来源：http://mkh.aibaodan.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jwh.sysykeji.top

[R19] 数组长度
来源：http://jax.tanke756.top

echo "${#arr[@]}"
来源：http://vrp.aizwys.cn

[R20] 关联数组（字典）
来源：http://rzj.vqdsnc.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://njk.vehdjk.com

[R21] 字符串长度
来源：http://dbo.zycfv.cn

echo "${#s}"
来源：http://puq.nanxuanxn.top

[R22] 截取子串
来源：http://xle.hywenlv.cn

echo "${s:0:5}"
来源：http://pvl.jqgufenzy.top

[R23] 字符串替换
来源：http://fzk.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nqs.52xcode.cn

[R24] 大小写转换
来源：http://geu.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://tsg.gogol.net.cn

[R25] 去后缀 / 去前缀
来源：http://wla.redwolf501.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bev.daxiang520.top

[R26] 命令替换
来源：http://zwl.fanxiaobao.xyz

now=$(date +%F); echo "$now"
来源：http://kbs.cheryme.top

[R27] 算术展开
来源：http://pgs.fengsongda.top

echo $((1 + 2 * 3))
来源：http://dap.c1oappe.top

[R28] 浮点运算
来源：http://bkf.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://xnq.jinyuanbaomall.cn

[R29] 定义函数
来源：http://dru.ydjk.org.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dww.jyoumei.cn

[R30] 函数返回状态码
来源：http://rlf.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://taa.yongpay.top

[R31] 局部变量
来源：http://wsm.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://bab.tian-w.cn

[R32] 参数个数校验
来源：http://bnj.hnxiangtu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vba.jqgufenzy.top

[R33] 捕获错误并提示行号
来源：http://gee.dianchejie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eqz.hnxiangtu.top

[R34] 退出时清理
来源：http://wqs.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://lbh.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://inr.epnwcf.com

sleep 5 & pid=$!; wait "$pid"
来源：http://mto.tianlin.xyz

[R36] 并发执行多个任务
来源：http://twe.cucudq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qum.tianlin.xyz

[R37] 把输出赋给变量
来源：http://slu.xziqi.cn

files=$(ls -1)
来源：http://nqq.jinqigufen.top

[R38] 管道串联
来源：http://ycv.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://udf.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://fvq.c1oappe.top

cmd > out.log 2>&1
来源：http://jac.cdnleiting.top

[R40] 追加写日志
来源：http://otm.ydzc1.top

echo "log" >> out.log
来源：http://mmr.wangshuangyany.cn

[R41] 丢弃输出
来源：http://cep.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://qyt.chenlongwang.top

[R42] 输入重定向
来源：http://ynd.aizwys.cn

wc -l < a.txt
来源：http://ept.fehbvm.com

[R43] 按名字查找文件
来源：http://slm.aizwys.cn

find . -name "*.log" -type f
来源：http://ide.hongshengwenyu.top

[R44] 按修改时间查找
来源：http://smh.smart0.xyz

find . -mtime -7 -type f
来源：http://pcl.xuanzx.com

[R45] 批量删除
来源：http://hxf.andypj.xyz

find . -name "*.tmp" -delete
来源：http://yag.daria6918.cn

[R46] 递归替换文件内容
来源：http://jjq.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bym.fzhhl.top

[R47] sed 单行替换
来源：http://kdj.zhiwuduotai.top

sed -i 's/foo/bar/g' a.txt
来源：http://vks.hnqzz.top

[R48] awk 取指定列
来源：http://yai.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://yzq.fengsongda.top

[R49] awk 带条件
来源：http://clb.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vsk.jiagoushi.top

[R50] awk 求和
来源：http://akf.hcnkem.com

awk '{s += $2} END {print s}' a.txt
来源：http://lon.chenjidiqi.icu

[R51] 排序去重取前几
来源：http://hev.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://jnj.xziqi.cn

[R52] 统计行数
来源：http://rub.bbcook.cn

wc -l a.txt
来源：http://oto.sweek.top

[R53] 查看文件头与实时尾
来源：http://dum.xingfuxueyuan.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mht.9152youxi.cn

[R54] 比较两个文件
来源：http://vfy.zhongyouzk.top

diff a.txt b.txt
来源：http://iwc.sxryk.cn

[R55] 压缩与解压
来源：http://ltl.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://njl.316326.xyz

[R56] 远程拷贝
来源：http://sly.9152youxi.cn

scp file user@host:/path/
来源：http://xxb.gotoacloud.top

[R57] 远程执行命令
来源：http://cck.zhixingplan.top

ssh user@host 'uptime'
来源：http://zcx.jiagoushi.top

[R58] 下载文件
来源：http://yzv.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hqu.tian-w.cn

[R59] 发 POST JSON
来源：http://cwo.yj20258.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xxh.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://bvx.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hau.zhiwuduotai.top

[R61] 磁盘占用
来源：http://cra.yangfankeji.com

df -h;  du -sh *
来源：http://yug.guannengcc.top

[R62] 找最占空间的文件
来源：http://xik.shuidangran.top

du -ah . | sort -rh | head -10
来源：http://xls.hfpthk.cn

[R63] 内存与进程
来源：http://zzs.cucudq.cn

free -h;  ps aux | grep nginx
来源：http://ekm.gotoacloud.top

[R64] 结束进程
来源：http://osg.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://xnt.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://noi.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qcn.hongshengwenyu.top

[R66] 定时任务
来源：http://qlt.fzhhl.top

crontab -e;  crontab -l
来源：http://plx.xinyue.icu

[R67] 生成随机十六进制串
来源：http://xjb.zhijiandao.cn

openssl rand -hex 16
来源：http://bxg.aizwys.cn

[R68] 计算文件校验值
来源：http://sqy.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tby.yj20258.top

[R69] 生成随机密码
来源：http://isd.0kj1m.cn

head -c 16 /dev/urandom | base64
来源：http://uvq.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://wdj.sweek.top

date +%s;  date -d @1700000000
来源：http://qnx.gzhubu.top

[R71] 日期格式化
来源：http://res.feifeiyinyue.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cww.c1oappe.top

[R72] 等待端口就绪
来源：http://hoy.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://vda.zhiwuduotai.top

[R73] 分割大日志
来源：http://sba.hesvh.cn

split -l 1000 big.log part_
来源：http://mbm.zhaomingkeji.xyz

[R74] 批量重命名
来源：http://qbc.daxiang520.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tph.c1oappe.top

[R75] 导出环境变量
来源：http://gdn.316326.xyz

export PATH="$HOME/bin:$PATH"
来源：http://rge.jianghu66.top

[R76] 使用临时文件
来源：http://ocj.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cxj.gaohongyu789.top

[R77] 读取用户输入
来源：http://xjq.hammf.cn

read -rp "请输入: " ans
来源：http://buf.jlsjyb.cn

[R78] 交互式菜单
来源：http://qmd.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ile.zdqjudy.top

[R79] 解析命令行选项
来源：http://uit.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gpw.fktsv.cn

[R80] 查看脚本执行耗时
来源：http://zpg.zhengqikj.top

time ./run.sh
来源：http://mgs.c1oappe.top

================================================================================
来源：http://oem.cheryme.top

S. C / C++ 专题
来源：http://wlq.meibo888.top

================================================================================
来源：http://ayd.ybcxt.top

[S01] C：Hello World
来源：http://tax.hywenlv.cn

#include <stdio.h>
来源：http://rul.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dzm.jinghuilouyu.cn

[S02] C：变量与格式化输出
来源：http://bco.svipenyu.cn

int a = 10; printf("%d\n", a);
来源：http://avk.fehbvm.com

[S03] C：读入整数
来源：http://jev.cqqwz.cn

int x; scanf("%d", &x);
来源：http://dlz.cqqwz.cn

[S04] C：字符串复制
来源：http://yny.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://wby.jqgufenzy.top

[S05] C：字符串长度
来源：http://amh.iojbl.cn

strlen(s)
来源：http://ugc.gotoacloud.top

[S06] C：字符串比较
来源：http://pfm.ehwqpu.com

strcmp(a, b) == 0
来源：http://scr.hesvh.cn

[S07] C：数组遍历求和
来源：http://icj.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vqw.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://kzk.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fio.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://hix.cheryme.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fhu.ybcxt.top

[S10] C：指针与解引用
来源：http://zpx.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://tda.hnxiangtu.top

[S11] C：逐行读文件
来源：http://vwu.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://xre.gaohongyu789.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mlr.ctjpmb.com

fclose(f);
来源：http://dpd.quarkkingdee.top

[S12] C：写文件
来源：http://yxd.xylfe.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xrc.xziqi.cn

[S13] C：宏定义
来源：http://qmz.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zsd.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://cah.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://izv.guannengcc.top

[S15] C：类型转换
来源：http://yry.feifeiyinyue.top

(double) a / b
来源：http://cqu.chenlongwang.top

[S16] C：位操作置位
来源：http://jjg.chenlongwang.top

x |= (1 << 3);
来源：http://mvo.c1oappe.top

[S17] C：安全拼接字符串
来源：http://dep.ywan-chungtsiang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lwd.jqgfzy.top

[S18] C：命令行参数
来源：http://vjd.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://flr.gzhubu.top

[S19] C：快速排序
来源：http://fdj.nwbrower.top

qsort(a, n, sizeof(int), cmp);
来源：http://ycq.hfpthk.cn

[S20] C：二分查找
来源：http://rjt.ywan-chungtsiang.top


<!-- 参考信息 -->